- If we want to set environment variables in Vim without contaminating the environment variables in our system. Just declare them only in the `.vimrc` like below.
  
  ```bash
  let $FZF_DEFAULT_COMMAND = 'rg --files'
  ```
- `tags`: #VIM