# setup_repo
Repo with useful information for setuping environment.

# Winget
Download [Winget (Windows 10)](https://apps.microsoft.com/store/detail/instalador-de-aplicativo/9NBLGGH4NNS1).

## Using Winget to install apps
First of all, search for the app_name at the winget repository typing this command at Command Prompt or PowerShell:
```
winget search [app_name]
```
After finding the correct app, get its id and type the following:
```
winget install [app_id]
```

# Terminal
Download [Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701).

For extra customization, use [oh My Posh](https://ohmyposh.dev).

# WSL
If you are at Windows 11 or an recent build of Windows 10, type this at PowerShell:
```
wsl --install
```

If you are at an older Windows 10 build use this [tutorial](https://learn.microsoft.com/windows/wsl/install-manual).

## Docker
Download [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/).

After installing Docker, remember to enable WSL2 inside it. Open up Docker Desktop, go to **Settings>Resources>WSL Integration** and enable the WSL2 integration.

# Git
Download [Git Bash](https://git-scm.com/download/win).

After installation, open up Git Bash or Linux Terminal and configure yout username and e-mail:
```
git config --global user.name [username]
git config --global user.email [email]
```
Then, create your ssh key:
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
Or:
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
Copy your public ssh key by typing:
```
clip < ~/.ssh/[key_name].pub
```
Now, add the public ssh key to Github by entering **Settings>SSH and GPG keys** and pasting the key. Remember to do the same for the WSL distro.

# Visual Studio Code
## Extensions
- Material Icon Theme
- Dracula Official Theme
- Remote-SSH
- WSL
- Live Server

# Useful Apps
- Notepad++
- DBeaver

# Useful Tips
- [Creating local instance MySQL using Docker](/utils/mysql_docker_setup.md)

# To be added:
- Windows Terminal Configs
- VSCode Configs