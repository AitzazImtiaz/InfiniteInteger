<p align="center"><img src="https://img.shields.io/badge/INFINITE%20-INTEGER-blue?style=for-the-badge&logo=appveyor" height="50"></p>
<p align="center"><img src="https://img.shields.io/github/issues/AitzazImtiaz/InfiniteInteger?style=social&logo=appveyor"><img src="https://img.shields.io/github/forks/AitzazImtiaz/InfiniteInteger?style=social&logo=appveyor"> <img src="https://img.shields.io/github/stars/AitzazImtiaz/InfiniteInteger?style=social&logo=appveyor"><img src="https://img.shields.io/github/license/AitzazImtiaz/InfiniteInteger?style=social&logo=appveyor"> <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Fgithub.com%2FAitzazImtiaz%2FInfiniteInteger"></p>

The following is a ```.dll``` of [InfInt.h](https://github.com/sercantutar/infint/blob/master/InfInt.h) which was made by Sercantutar, this compiled file has the ability of working with Infinite Integers. Although, the library does have drawback, it does not support any cross-variable types, so can not run simultaneously with ```long long``` ```int``` or anything. Now, you can create any Windows Application using this ```.dll``` that can support infinity of numbers! 

Here is a sample code:
```
#include <iostream>
#include "InfiniteInteger.h"

using namespace std;

int main(){
  InfInt myint1 = "15432154865443143186646848435145841005101684046451560358";
  InfInt myint2 = 156341300544608LL;

  myint1 *= --myint2 - 3;
  cout << myint1 << endl;
  
  return 0;
}
```

The InfInt.h repository also cites something, that is practically possible in Infinite Integer library.
<blockquote>
Useful methods:

    intSqrt: integer square root operation
    digitAt: returns digit at index
    numberOfDigits: returns number of digits
    size: returns size in bytes
    toString: converts it to a string

There are also conversion methods which allow conversion to primitive types:

    toInt, toLong, toLongLong, toUnsignedInt, toUnsignedLong, toUnsignedLongLong.

You may define INFINT_USE_EXCEPTIONS and library methods will start raising InfIntException? in case of error instead of writing error messages using std::cerr.
</blockquote>

The instructions [here](https://www.learncpp.com/cpp-tutorial/a2-using-libraries-with-visual-studio-2005-express/) are really helpful for running this code on Windows.
