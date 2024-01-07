# Use clang-format and clang-tidy in VS code

Paste the following settings in the JSON file of VS Code.

```text
{
  /*-------------------- GLOBAL EDITOR CONFIGURATIONS -------------------------*/
  "editor.formatOnType": false,
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  // "editor.defaultFormatter": "llvm-vs-code-extensions.vscode-clangd",
  /*----------------------------- C++ STUFF ----------------------------------*/
  "C_Cpp.autocomplete": "disabled",
  "C_Cpp.formatting": "disabled",
  "C_Cpp.errorSquiggles": "disabled",
  "C_Cpp.intelliSenseEngine": "disabled",
  //clangd
  // "clang-tidy.enabled": false,
  "clangd.arguments": [
    "--background-index",
    "--clang-tidy",
    "--header-insertion=never",
    "--suggest-missing-includes",
    "--compile-commands-dir=build/"
  ],
  "clangd.path": "/usr/bin/clangd",
  "C_Cpp.default.cppStandard": "c++17",
  "editor.inlayHints.enabled": "off",
  // "C_Cpp.clang_format_path": "/usr/bin/clang-format",
  // "C_Cpp.clang_format_style": "file:/slambook-en_notes/.clang_format",
  // "C_Cpp.clang_format_sortIncludes": true,
  // "C_Cpp.codeAnalysis.clangTidy.path": "/usr/bin/clang-tidy",
  // "markdown-preview-enhanced.liveUpdate": false,
  // "C_Cpp.codeAnalysis.clangTidy.codeAction.formatFixes": false,

}
```
