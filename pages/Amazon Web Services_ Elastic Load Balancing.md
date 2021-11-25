## Overview
	- The Elastic Load Balancing automatically distributes incoming traffic across multiple targets, such as EC2 instances, containers and IP addresses.
		- Monitor the health of registered targets and routes traffic only to the healthy targets.
		- It can automatically scale to the vast majority of workloads.
	- Supports Application Load Balancers (ALB), Network Load Balancers (NLB), Gateway Load Balancers (GLB) and Classic Load Balancers (CLB).
## Classic Load Balancer
![2021_11_25_image.png](https://cdn.logseq.com/%2F2309e0bd-62fc-484d-ae20-c099c4a388c01d482d2e-378d-4233-8267-01844d4366352021_11_25_image.png?Expires=4791379297&Signature=gLlc7~jkQBrM3p8S5PgFe0S42qWcYEkXUKE7k0PAN~8h735GoHRoeYrmPvXdjGT-GJKawI3E7ZX2jrdLgiluuTIvXn9sDyL-2vd9aoKyzdPyDIRYpMxwws9u9AjW~8EaeG9rVjOVXUtUfaOTiV7Ut6nP4eVjME9cZJ7uJAo9IcoGzopRwKw1P9NDT-r6UvB1txy2stIK2iEGlzAJprwQvgvECmceNbTcvQoRk5IUdQLfAlNyMT8ANjfN31H~vknt41Gs8-LxLK9guodN9hOoVvK0olpmHRBDsW0h4lwUUK5UiIgvBK4ZCgntkyNRP4SVSsffQTa5tUWZMklaOVrrOw__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA)
	- The load balancer serves as a single point of contact for clients.
	- We can add and remove instances from the load balancer as our needs change.
	- A listener checks for connection requests from clients, using the protocol and port that we configure, and forwards requests to one or more registered instances.
	- We can configure health checks, which are used to monitor the health of the registered instances.