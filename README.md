# Auto Region Folder for Visual Studio Code

This extension folds all regions automatically when open files in Visual Studio Code.

## Example of appearance

### C++

#### Before

```c++
#pragma region header

#include <bits/stdc++.h>
#define rep(i, n) for (int i = 0; i < (int)(n); i++)
using namespace std;

#pragma endregion header

int main() {
  rep(i, 42) cout << i << endl;
}

```

#### After

```c++
#pragma region header

int main() {
  rep(i, 42) cout << i << endl;
}

```

### Markdown

#### Before

```md

- main content

<!-- #region trivial -->

- trivial content

<!-- #endregion trivial -->
```

#### After

```md

- main content

<!-- #region trivial -->
```

### etc

See [The official docs](https://code.visualstudio.com/docs/editor/codebasics#_folding).

## Practical test

Open this file with Visual Studio Code and see the following region.

<!-- #region test -->

### Test region

- This region is automatically folded.

- On the contrary, the region within the above code block of Markdown is not folded.

<!-- #endregion test -->

## Author

- **[dnek](https://github.com/dnek)**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.