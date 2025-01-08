How to Create a Virtual Environment
===================================

Virtual environments are essential for isolating project dependencies and ensuring compatibility across different projects. This guide explains how to create a virtual environment using Python's built-in `venv` module.

Prerequisites
-------------
- Python 3.3 or newer installed on your system.
- A terminal or command prompt to execute commands.

Steps to Create a Virtual Environment
-------------------------------------

1. **Open a Terminal or Command Prompt**
   Open the terminal (or Command Prompt on Windows) and navigate to the directory where you want to create the virtual environment.

2. **Run the Command**
   Execute the appropriate command based on your operating system:

   - **On Windows**:
      .. note::

      -m venv myenv

   - **On macOS/Linux**:
      .. note::

      -m venv myenv

   Replace `myenv` with the name of your virtual environment directory.

3. **Verify the Creation**
   After running the command, a new directory (e.g., `myenv`) will be created in your current location. This directory contains the files needed for the virtual environment.

Understanding the Structure
---------------------------
The virtual environment directory contains:
   - **`bin` or `Scripts`**: Contains the executables, including the Python interpreter.
   - **`lib`**: Includes the standard library and site packages for your virtual environment.
   - **`pyvenv.cfg`**: Configuration file for the virtual environment.

Next Steps
----------
Once created, you can activate the virtual environment. Refer to the guide on **fill this in with the link to the other guide you made pls**

