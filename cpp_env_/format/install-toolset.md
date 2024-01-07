# Installing my toolset for C++

I will use the following toolset:

- git
- build tools
- cmake
- cppcheck
- clang-tools
- clang-format
  
```bash
sudo apt update
sudo apt install -y git build-essential cmake cppcheck clang-format clang-tidy clangd
```

## Install VS Code extensions

Visual Studio Code Extension Summary

### C++

|Name |How to install: Ctrl + p and type|
|-------|-------------------------------------------------|
|C/C++ |ext install ms-vscode.cpptools|
|clangd |ext install llvm-vs-code-extensions.vscode-clangd|

### CMake

|Name| How to install: Ctrl + p and type|
|-------|-------------------------------------------------|
|CMake| ext install twxs.cmake|
|CMake Tools Helper| ext install ms-vscode.cmake-tools|
|CMake format| ext install cheshirekow.cmake-format|

Run the following commands:

```bash
code --install-extension ms-vscode.cpptools
code --install-extension llvm-vs-code-extensions.vscode-clangd
code --install-extension twxs.cmake
code --install-extension ms-vscode.cmake-tools
code --install-extension cheshirekow.cmake-format
code --install-extension yzhang.markdown-all-in-one
code --install-extension DavidAnson.vscode-markdownlint
```

## Sources

- [github repo: must-have-tools from nachovizzo](https://github.com/nachovizzo/must-have-tools/wiki)
