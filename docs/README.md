# Awesome OS Setup
![Logo](images/logo.png)


| Windows WSL Terminal                                     | Desktop with terminals                                        |
|----------------------------------------------------------|---------------------------------------------------------------|
| ![Windows WSL Terminal](images/windows_wsl_terminal.png) | ![Desktop with terminals](images/desktop_with_terminals.jpeg) |


<div style="text-align: center;">The image you are looking at is a screenshot of a WSL Ubuntu terminal in Windows 11. The top bar is an app called GlazeWM which is a a tiling WM that lets you organize windows and adjust their layout on the fly by using keyboard-driven commands.
You can follow this repository to get a similar setup on Windows11, Linux or both.

![Windows 11](https://img.shields.io/badge/Windows%2011-%230079d5.svg?style=for-the-badge&logo=Windows%2011&logoColor=white)
[![Linux](https://img.shields.io/badge/-Linux-grey?style=for-the-badge&logo=linux)](https://www.microsoft.com/en-in/windows)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white)
![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white)
</div>

## Linux/WSL2
A set of configurations,
dotfiles and a script to automatically set up a powerful terminal & shell utilities(zsh,fzf, ctrl+f on terminal to search files & folder...),
themes like Powerlvl10k, Conda, GPU drivers, and more on Linux/WSL2, again automatically.

Get started with one command :
```bash
sh -c "$(wget https://raw.githubusercontent.com/AmineDjeghri/awesome-os-setup/main/docs/unix_workflow/auto_linux_setup.sh -O -)"
```
Read more about it here: [README](unix_workflow/README_unix.md) / [website](https://setup.aminedjeghri.com/readme-unix.html)

## Windows 11/WSL2
Valuable applications & tips for enhancing your Windows user experience, with a focus on creating a productive environment incorporating WSL 2 (Linux).

Read more about it here: [windows_workflow_README.](windows_workflow/README_windows.md) / [website](https://setup.aminedjeghri.com/readme-windows.html)

**Browser extensions**
Read more about it here: [browser_extensions.md](windows_workflow/browser_extensions.md) / [website](https://setup.aminedjeghri.com/browser-extensions.html)

**For Windows users: Why you should use WSL2?**
WSL2 enables users to run Linux applications and utilize command-line tools natively on their Windows machines.
This integration allows users
to enjoy the familiarity of Windows while simultaneously harnessing the power and flexibility of Linux.

|              | macOS                                                                         | Linux                                                                      | Windows with WSL                                                                                                                                                                                                                          |
|--------------|-------------------------------------------------------------------------------|----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Advantages   | (+) Excellent for coding and video editing. Supports Adobe & Office products. | (+) Ideal for coding and gaming, providing good performance in both areas. | - (+) Seamless compatibility with diverse software, including Adobe & Office products. </br> (+) Optimal choice for gaming enthusiasts </br> (+) Well-suited for coding with Windows Subsystem for Linux (WSL) and no need for dual boot. |
| Inconvenient | (-) Limited gaming capabilities compared to Windows & Linux.                  | (-) Lacks support for Adobe & Office products and certain software.        | (-) UI is not smooth and responsive compared to macOS & Linux                                                                                                                                                                             |


Within the domain of development, Unix-based systems such as Linux and macOS frequently garner attention. Nevertheless, the integration of WSL allows smooth coding alongside the utilization of Adobe and Microsoft products that may lack support on Linux. This flexibility, coupled with the ability to handle resource-intensive games beyond macOS capabilities, positions Windows-WSL as an enticing platform, ensuring a well-rounded computing experience for all users, regardless of their workplace constraints.

Based on your needs, you can choose your OS.

## Contributing
- Git clone the repository
- Install and run pre-commit to check the code before pushing it with :
  - `pip install pre-commit`
  - `pre-commit install`
  - `pre-commit run --all-files`

- Generated docs:
    A folder named `docs` contains the docs for generating the website with Jetbrains Writerside plugin.
    Writerside supports only one file named `README.md`
    that's why you will find other readme files like `unix_workflow/README_unix.md`
    instead of being named `unix_workflow/README.md`.
-  Modifying dotfiles like `.zshrc`:
  - use `stow` to create symlinks to the dotfiles in your home directory as follows:
  - `cd docs/unix_workflow/` then ``stow -t $HOME -R dotfiles ``
  - this will create symlinks to the dotfiles in your home directory: ``cd ~ && cat .zshrc``
  - WARNING: Windows users can't open the dotfiles in their home directory with their text editor, you can only with the terminal or open them in the repo folder.

**Star History Chart**
[![Star History Chart](https://api.star-history.com/svg?repos=aminedjeghri/awesomewindows11&type=Date)](https://star-history.com/#aminedjeghri/awesomewindows11&Date)