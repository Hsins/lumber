title:: The LBYL Style v.s. The EAFP Style

## LBYL (Look Before You Leap)
	- This coding style explicitly tests for pre-conditions before making calls or lookups. This style contrasts with the EAFP approach and is characterized by the presence of many if statements.
	- In a multi-threaded environment, the LBYL approach can risk introducing a race condition between “the looking” and “the leaping”. For example, the code, `if key in mapping: return mapping[key]` can fail if another thread removes key from mapping after the test, but before the lookup. This issue can be solved with locks or by using the EAFP approach.
## EAFP (Easier to Ask for Forgiveness Than Permission)
	- This common Python coding style assumes the existence of valid keys or attributes and catches exceptions if the assumption proves false. This clean and fast style is characterized by the presence of many `try` and `except` statements. The technique contrasts with the LBYL style common to many other languages such as C.
## References
	- [程式語言文化差異 LBYL v.s. EAFP | Medium](https://medium.com/little-sunshine/%E7%A8%8B%E5%BC%8F%E8%AA%9E%E8%A8%80%E6%96%87%E5%8C%96%E5%B7%AE%E7%95%B0-lbyl-v-s-eafp-342da64277f3)