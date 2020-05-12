# Optimized Lua

Modified source code of Lua 5.3.5 tuned for performance.

![Lua logo](http://www.lua.org/images/lua-logo.gif)


# Optimizations

* tuned compiler flags:
  * set optimization level 3 (-O3)
  * enable link time optimization (-flto)
  * enable all instruction subsets supported by the local machine (-march=native)


# Other modifications

There are other modifications related to building the code in different environments.


# Tested environments

* Apple clang version 11.0.3 (clang-1103.0.32.59) on macOS Catalina


# Author

André Pereira Henriques [aphenriques (at) outlook (dot) com].


# Donation

* BTC: 1BdPza4JSYxKt4YAgPm579ZEqK2hHQNfij
* ETH: 0xc8eD4EcCAd66BD928EB9B1696a05AeFf8DBA699e


# Further information

For installation instructions, license details, and
further information about Lua, see doc/readme.html.
