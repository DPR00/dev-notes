# Install VS code

## 1st option

Download it from snap

```bash
sudo snap install -y code --classic
```

## 2nd option

- Download .deb package from [VS Code page](https://code.visualstudio.com/)
- Install it from Ubuntu Software or from terminal
  
    ```bash
    sudo apt install -y ./<file>.deb
    ```

## 3rd option

Run the following commands

```bash
sudo apt update
sudo apt install software-properties-common apt-transport-https wget -y
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install -y code
```

## Sources

- [phoenixNAP](https://phoenixnap.com/kb/install-vscode-ubuntu)
