---
title: New Member Setup
---

Here are instructions on how to install devtools. This includes some instructions for installing platform-specific toolchains and IDEs, along with general installation instructions for other software. Chances are you already have some of these tools installed already!

---

## Platform-specific

### MacOS (10.7+)

<details>
<summary>Instructions</summary>

#### JUCE

- Go to the [JUCE download page](https://juce.com/get-juce/download)
- Select the "Mac" button to download the latest version of the library with tools pre-built for MacOS
- Expand the `.zip` file by double-clicking in Finder or running `unzip ./juce-7.x.x-osx.zip` in terminal
- Move the new `JUCE` folder to `/Users/<your username>/Applications` in Finder or in terminal running `mv -r ./JUCE ~/Applications/` in the directory you expanded it in.

#### XCode

- Go [to the MacOS App Store](https://apps.apple.com/us/app/xcode/id497799835?mt=12) to install the XCode app
- Open the terminal (`/System/Applications/Utilities/Terminal.app`) and run `xcode-select --install` to install the XCode command line tools
  - this will install the compiler, linker, debugger, etc.

#### Python3

[This guide](https://docs.python-guide.org/starting/install3/osx/) is simple and avoids conflicting installations.


</details>

### GNU/Linux (Kernel version 4.x or 5.x, recent version of a mainstream distro)

<details>
<summary>Instructions</summary>

__TODO__

</details>

### Windows (10+)

<details>
<summary>Instructions</summary>

#### JUCE

- Go to the [JUCE download page](https://juce.com/get-juce/download)
- Select the "Windows" button to download the latest version of the library with tools pre-built for Windows
- Select the `.zip` archive in File Explorer and select "Compressed Folder Tools"->"Extract All"
- Extract the JUCE folder inside your home directory, i.e. "C://Users/\<your username\>/", removing the name `juce-x.x.x-windows` from the path.

#### Visual Studio (a.k.a. not VSCode)

- Follow Microsoft's instructions [here](https://docs.microsoft.com/en-us/visualstudio/install/install-visual-studio?view=vs-2022)
  - The community version of Visual Studio is preferable
  - For workload, you'll want to select the "Desktop Development with C/C++" one.

#### Git

[This article](https://www.makeuseof.com/install-git-git-bash-windows/) is pretty clear: skip to the section "Download and Install Git for Windows."

#### Python3

- Navigate to [the Python website](https://www.python.org/downloads/windows/) and go to the first link titled "Latest Python 3 Release." Download the recommended 64-bit Windows installer executable.
- Open the Python3 installer
  - select "Add Python 3.x to PATH" so you can use python on the command line. For reference, the command will be `python`
  - select "Install Now" and follow the installer's instructions

</details>

---

## General stuff

### Installing and Configuring Git/GitHub

Git should be pre-installed on Linux and comes with the [XCode CLI Tools on MacOS, described above](#XCode). Follow the instructions [above](####Git) for Windows.

- To authenticate with GitHub, the easiest way now is to use the GitHub CLI tool. [These instructions by GitHub] tell you how to do that for Mac, Windows, and Linux.
  - _Alternatively, you can manually generate an SSH key or PAT for your GitHub account without installing the CLI tool. In that case, follow [these instructions by GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)_
- Then, run `gh auth login` in a terminal to login to your github account

### IPython/Jupyter Notebook

### Testing your JUCE installation

