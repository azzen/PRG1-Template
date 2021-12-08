## Compiler flags

```
-Wall -Wextra -Wconversion -Wsign-conversion -pedantic
```

## Recommended code style

 - Maximum of **85 columns** per line of code.
 - Use tabs instead of spaces.
 - Every file of the project must have at the top, the provided header

 ```
 /*
 -----------------------------------------------------------------------------------
 Nom du fichier : <file name>
 Auteur(s)      : <author(s)>
 Date creation  : <creation date>
 Description    : <file description>
 Remarque(s)    : <remark, algorithm descriptions, references, etc.>
 Compilateur    : <compiler and version, e.g. Mingw-w64 g++ 11.2.0>
 -----------------------------------------------------------------------------------
*/
 ```

- Comments and identifiers must be in French, you'll have the opportunity to write in English in other courses.

General advice:
> Be consistent throughout your code, as long as you keep the same code style across your different files, there's a high chance that you won't be evaluated negatively.

<hr/>

Constants:  upper case and use underscores as separators. Avoid using preprocessor directives such as `#define`.

```cpp
const int MY_CONSTANT = 42;
```

Variables identifiers: camelCase.

```cpp
int myVariable = 42;
```

Function names and parameters: camelCase.

```cpp
Matrix& myFunction(int n, int m, string& matrixName = "Test");
```

Custom types: use `using` instead of `typedef`, identifiers should be written in PascalCase.

```cpp
using Matrix = vector<vector<double>>;
```

Use `auto` when it helps for the code readability, e.g. for iterators.

```cpp
#include <vector>
using namespace std;

vector<int> v = { 1, 2, 3 };
for (auto i = v.begin(); i != v.end(); ++i) {
    cout << *i << endl;
}
```

<hr>

todo: generics, object-oriented, exceptions, enums



