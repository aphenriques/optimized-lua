# Optimized Lua

Modified source code of Lua 5.3.6 and Lua 5.4.6 tuned for performance.

![Lua logo](http://www.lua.org/images/lua-logo.gif)


# Optimizations

* tuned compiler flags (Lua 5.3.6 and Lua 5.4.6):
  * set optimization level 3 (-O3)
  * enable link time optimization (-flto)
  * enable all instruction subsets supported by the local machine (-march=native)
* computed goto (Lua 5.3.6) (stock Lua 5.4.6 implements it by default):
  * Miro Knejp's https://github.com/mknejp/computed-goto
  * check out his excelent talk ["Non-conforming C++: the Secrets the Committee Is Hiding From You" on CppCon 2019](https://youtu.be/IAdLwUXRUvg) where he explains computed goto starting on [31:17](https://youtu.be/IAdLwUXRUvg?t=1877) (Lua implementation starts on [40:12](https://youtu.be/IAdLwUXRUvg?t=2412))


# Other modifications

There may be other modifications related to building the code in different environments.


# Tested environments

* Apple clang version 11.0.3 (clang-1103.0.32.59) on macOS Catalina
* gcc 10.1.1 on [Clear Linux OS](https://clearlinux.org)

# Author

André Pereira Henriques [aphenriques (at) outlook (dot) com].

Most of the work of the techniques employed in this repository were done by others. See each optimization on [Optimizations](#optimizations) for the references.
