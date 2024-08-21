# Python Environemnt Test

Welcome to the Python Environemnt Test! This repository will walk you through the steps to clone the repository, set up the environment using `uv`, and use the project within Visual Studio Code (VSCode).

## Prerequisites

Before you begin, ensure you have the following installed on your system:

1. **Git**: To clone the repository.
2. **Python**: Make sure Python is installed. You don't need the exact version specified by the project; `uv` will handle that.
3. **VSCode**: The recommended code editor for this project.
4. **Python Extension for VSCode**: This extension provides features like linting, debugging, and IntelliSense.

### Install Git
If Git is not installed, you can download and install it from [here](https://git-scm.com/downloads).

### Install Python
If Python is not installed, you can download and install it from [here](https://www.python.org/downloads/). You don't need the exact version specified by the project; `uv` will handle that.

### Install VSCode
If VSCode is not installed, you can download and install it from [here](https://code.visualstudio.com/).

### Install Python Extension for VSCode
Open VSCode, go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window, and search for "Python". Click "Install" to add the extension.

## Step 1: Clone the Repository

Start by cloning the repository to your local machine:

```bash
git clone https://github.com/yutawatabe/python_environment_test.git
cd my_project
```

## Step 2: Install uv

If you don't have uv installed, you can install it via pip:

```bash
pip install uv
```

## Step 3: Set Up the Environment with uv

Now, use uv to set up the project environment:

```bash
uv setup
```

This command will:

- Download and install the correct Python version specified in the pyproject.toml file.
- Install all necessary packages and dependencies into an isolated environment located in the .uv directory.

## Step 4: Open the Project in VSCode

Launch VSCode and open the project folder:

### Select the Python Interpreter

1. Press Ctrl+Shift+P (or Cmd+Shift+P on macOS) to open the Command Palette.
2. Type Python: Select Interpreter and press Enter.
3. Select the interpreter located in the .uv directory. It should be something like:

```bash
.uv/bin/python
```

## Step 5: Activate the Environment
In VSCode's integrated terminal:
- Open a new terminal by pressing `Ctrl+`` (backtick).
- Activate the uv environment:

```bash
source .uv/bin/activate
```

This activates the isolated environment where all dependencies are installed.

## Step 6: Run and Debug the Code

With the environment set up and activated, you can now run and debug the code:
- Open any Python file from the src directory.
- Click the "Run" button (a green play icon) at the top right, or press F5 to start debugging.
- VSCode will use the uv environment, ensuring that the correct Python version and dependencies are in use.

