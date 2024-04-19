# Sign Language Detector Python

Sign language detector with Python, OpenCV and Mediapipe !

Credit to this video [![Watch the video]](https://www.youtube.com/watch?v=MJCSjXepaAM)

# Workshop 1: Look at the Bitcamp slides
Here is a link for the slides. Please take a look at this: [Github slides](https://docs.google.com/presentation/d/1pXe2rrhoDVUvtryA6I3aUcQHmM3yQxe-EuK8QjWuXmM/edit#slide=id.p)

# Workshop 2: Set up the repository and dependencies
## HEAVILY RECOMMEND ATTENDING THIS WORKSHOP IF INTERESTED IN THIS PROJECT. THIS MAKES TROUBLESHOOTING EASIER.
A repository is just a collection of code that you worked on and are storing it some place for others to see. For all projects, using Github and repositories is necessary for showing your progress over time and a history of all the updates you have worked on throughout your project. Below is some of the necessary dependencies. **WE ARE ASSUMING THAT YOU HAVE PYTHON AND PIP INSTALLED!** These are necessary to download the dependencies below. If you do not have them installed, please google how to install:

        1. Python
        2. Pyenv or Conda
        3. Pip
        4. Homebrew (optional but helpful)

It's recommended to use a virtual environment like points 2 and 3 above to manage dependencies. If installation isn't working, try `python3` or `pip3` instead. **How to install the venv (virtual environment is later below.**

### If you do **NOT** have "git" installed PLEASE INSTALL IT TOO. INSTRUCTIONS BELOW
#### Introduction

Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. This guide will walk you through the steps to install Git on your system.

#### Installation Steps

#### Windows
1. **Download Git Installer:** [Visit the official Git website](https://git-scm.com) and download the latest version of Git for Windows.
2. **Run the Installer:** Once the download is complete, run the installer by double-clicking the downloaded file.
3. **Configure Installation Settings:** Follow the installation wizard, selecting the desired options. The default settings are usually sufficient for most users.
4. **Complete Installation:** Once the installation is complete, you can verify the installation by opening a command prompt and typing: `git --version`. This should display the installed Git version.

#### macOS
1. **Install Git via Homebrew** (recommended): If you have Homebrew installed, you can install Git by running the following command in the terminal: `brew install git`
2. **Install Git from [Git website](https://git-scm.com):** Alternatively, you can download the latest Git installer for macOS from the official Git website.
3. **Run the Installer:** Once the download is complete, run the installer by double-clicking the downloaded file.
4. **Configure Installation Settings:** Follow the installation wizard, selecting the desired options. The default settings are usually sufficient for most users.
5. **Complete Installation:** After installation, you can verify Git installation by opening a terminal and typing: `git --version`. This should display the installed Git version.

#### Linux
1. Install Git via Package Manager:
**Ubuntu/Debian:**
```
sudo apt-get update
sudo apt-get install git
```
**Fedora:**
`sudo dnf install git`
**Arch Linux:**
`sudo pacman -S git`
2. **Complete Installation:** Once the installation is complete, you can verify Git installation by opening a terminal and typing: `git --version`. This should display the installed Git version.

Now that we have git, navigate to the folder/directory that you want your code to be located on your computer using the `cd [directory name here]` command. `cd` means "change directory", or switch into that folder. If you want to pop back/exit the folder, use `cd ..`. Using these commands, run this code to clone the repo and have the repo template on your computer:

`git clone https://github.com/BigThinkAI-UMD/BitCamp-Student`
[Link to repo to clone here](https://github.com/BigThinkAI-UMD/BitCamp-Student)

Also, here is a .zip file of all the data you will need to build the model. It is too large to directly add to the Github repo linked above, so please download it and keep it in the same folder/directory/workspace as the rest of your files. [UPDATED_Data.zip](https://drive.google.com/file/d/1VrKK2v_x-wAZJviP-K5dNdrRyJspyYm8/view?usp=sharing)

## Setup Python Virtual Environment (venv)

Setting up a Python virtual environment is essential to isolate your project's dependencies from the system-wide Python installation. Follow these steps to create and activate a virtual environment for this project:

### 1. Create Virtual Environment

Open a terminal or command prompt and navigate to your project directory. Then, execute the following command to create a virtual environment named `venv`:

`python -m venv venv` (Again try python3 if that doesn't work)

This command will create a folder named *venv* in your project directory, which will contain the Python interpreter and libraries specific to your project.

### 2. Activate Virtual Environment
Activate the virtual environment using the appropriate command based on your operating system:
**For Windows:**

`.\venv\Scripts\activate`

**For macOS and Linux:**

`source venv/bin/activate`

After activation, you should see (venv) prefixed in your terminal prompt, indicating that the virtual environment is active.

**ONCE DONE WORKING, YOU DEACTIVATE THE ENVIRONMENT BY RUNNING `deactivate`**

Now, it is time to install the necessary dependencies.

**Run `pip install -r requirements.txt`**