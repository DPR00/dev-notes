# Installing NVIDIA drivers

## Context

When I tried to use PyTorch with `cuda()` I got an error saying that I have no NVIDIA drivers installed. In fact, when I run `nvidia-smi` I got the same error.

Therefore, I found this way to install NVIDIA drivers on my Linux system (Ubuntu 20.04).

## Steps

1. Check for NVIDIA drivers:
    `sudo ubuntu-drivers list`
    You should see something like this:
   - nvidia-driver-###-server
   - nvidia-driver-###
  If you found this kind of drivers, then you can install it.
2. Switch PPA to global mirrros. You can do it opening the Software & Updates app, then change the *Download from* to *Main server*.
3. Update packages with: `sudo apt-get update`.
4. Install the drivers with `sudo ubuntu-drivers install`.
5. Run `sudo apt update && sudo apt updgrade -y` to update.
6. Reboot.'
7. You should be able to run the `nvidia-smi` command and get your GPU information.

***Disclaimer***: I made the mistake of only running the `sudo ubuntu-drivers install` command. It indeed installed the drivers, but my WiFi drivers were broken and I couldn't connect to the Internet. I couldn't even connect to an external screen. So, I suggest follow all the steps.

## Sources

- [ask Ubuntu: Install NVIDIA drivers witouth broke WiFi drivers](https://askubuntu.com/questions/1286738/no-wi-fi-settings-or-connection-after-switching-to-nvidia-graphics-driver#:~:text=I%20also%20faced%20exact%20missing%20iwlwifi%20issue)
