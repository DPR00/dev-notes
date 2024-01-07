# Use black formatter extension for Python

Install the VS code extension: Black Formatter

```bash
code --install-extension ms-python.black-formatter
```

Add the following configuration to your JSON file

```text
  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter",
    "editor.formatOnSave": true
  }
```
