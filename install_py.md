# How to install python on Windows

I will teach you a way a little bit different from the traditional way to install python on Windows. This way is more practical and easy to use.
And the most thing will be done by the command line and ipynb file.

## Setting Up Anaconda Virtual Environment

Anaconda is a powerful tool for managing virtual environments and dependencies. Shiny apps can be run in isolated environments to manage package versions and dependencies efficiently.

1. **Install Anaconda***: To download and install Conda on Windows (or macOS), you'll typically use Miniconda or Anaconda, which are free distributions that include Conda, Python, and over 150 scientific packages and their dependencies.

**Visit the Official Anaconda Website**: Go to the Anaconda distribution page ([https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)) to download Anaconda or go to the Miniconda page ([https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)) to download Miniconda. Anaconda includes a lot of pre-installed packages which is useful for scientific computing, data science, and machine learning tasks. Miniconda is a minimal installer for Conda and you install the packages you need manually.

**Choose the Installer**: Select the Windows version of the installer. For Anaconda, you can choose between a graphical installer and a command-line installer. For Miniconda, download the appropriate .exe file.

**Run the Installer**: Once downloaded, double-click the installer to start the installation. Follow the instructions on the screen. It's recommended to check the option that adds Conda to your PATH environment variable, although the installer advises against it for beginners.

**Verify Installation**: Open the Command Prompt (cmd) and type `conda --version`. If Conda is installed, you should see the version of Conda printed on the screen.


2. **Create a New Virtual Environment**: After installing, you can use the `conda` command to manage packages and environments. For example, to create a new environment named `myenv` with Python 3.10, you would use:

```bash
conda create --name myenv python=3.10
```

3. **Activate the Virtual Environment**: Once the environment is created, activate it using:

```bash
conda activate myenv
```

## Step 3: Install Python package and find the Python path

Now in the Command Prompt (cmd) you should see something like:

```bash
(myenv) C:\Users\Desktop\...>
```

1. **Find Python path**: Then use `where python` to find python path:

```bash
where python
```
You should have somoe line like:

```bash
C:\Users\anaconda3\envs\myenv\python.exe
C:\Users\anaconda3\python.exe
C:\Users\AppData\Local\Microsoft\WindowsApps\python.exe
```
We gonan use the first path `C:\Users\anaconda3\envs\myenv\python.exe`.
