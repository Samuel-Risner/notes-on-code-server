# Extensions

- For compiling: `formulahendry.code-runner`
- For linting: `llvm-vs-code-extensions.vscode-clangd`

You might have to change the extension settings in `llvm-vs-code-extensions.vscode-clangd` by setting the paths for the clangd executable to `/usr/bin/clangd`.

# Dockerfile

If everything worked these commands should run:

```shell
gcc -v
g++ -v
clang -v
```
