## C++ pretty printer

forked from: [louisdx/cxx-prettyprint](https://github.com/louisdx/cxx-prettyprint)

A pretty printing library for C++ containers.

## Synopsis

Simply by including this header-only library in your source file,
you can say "std::cout << x" for any container object x. Sensible
defaults are provided, but the behaviour (i.e. the delimiters) are
compile-time customizable to a great extent via partial specializiation.

## Usage

Just:

``` bash
wget https://github.com/fATwaer/pretty-printer/blob/master/printer.hpp
```

Then:

``` c++
#include "printer.hpp"
#include <vector>

using namespace std;

int main() {
  vector<int> vec1 {0, 1, 2, 3, 4};
  cout << "vec1: " << ToString(vec1) << endl;

  map<int, string> mp1 {{42 , "answer"}, {1024 , "2^10"}};
  cout << "mp1: " << ToString(mp1) << endl;
}
```

Output:
```
vec1: [0, 1, 2, 3, 4]
mp1: [1: ["11", "12", "13"], 2: ["21", "22"], 3: ["31"]]
```

For details, please see the website (http://fatwaer.github.com/prettyprinter/).

License: Boost Software License, Version 1.0. See http://www.boost.org/LICENSE_1_0.txt.
