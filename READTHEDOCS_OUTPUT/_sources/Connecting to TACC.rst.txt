Connecting to TACC
==================

All these tutorials will be configured to work specifically on TACC systems so before we proceed, here is a quick tutorial on how to access and work on TACC's systems.

Prerequisites
-------------
1. **TACC Account**  
    - Ensure you have an active TACC account.  

2. **SSH Client**  
    - **Linux/macOS**: Use the built-in terminal.  
    - **Windows**: Use Windows Terminal.

Connecting to TACC
------------------
**Step 1: Open Your Terminal**  
   - On Linux/macOS, open the built-in terminal.  
   - On Windows, open your Windows Terminal.

**Step 2: Run the SSH Command**  
Use the following command to connect to TACC systems (replace `<username>` with your TACC username and `<hostname>` with the system hostname):

:: 

    ssh <username>@<hostname>

**Example:**
To connect to the Frontera system:

::

    ssh username@frontera.tacc.utexas.edu

**Step 3: Enter Your Password**  
When prompted, type your TACC password. If this is your first time logging in, you may be required to set up or reset your password.

**Step 4: Set Up Two-Factor Authentication (if required)**  
Some TACC systems require two-factor authentication. Follow the on-screen prompts to complete the process.

Tips and Troubleshooting
------------------------
- If you cannot connect, verify your username, hostname, and network settings.
- Contact TACC support if you encounter issues: `<https://portal.tacc.utexas.edu/help/>`_

Directories Explained
---------------------

While working on TACC systems, there are 3 main directories that users will utilize. $HOME, $WORK, and $SCRATCH. Understanding the difference between the three are quite simple: 
- $HOME: Useful for projects needing small environments as $HOME does not have much storage
- $WORK: Useful for general projects ...continue
- $SCRATCH: Useful for work that may be discarded as this directory may get purged

However, a potential issue with $WORK is that is you have a very large environment...continue

Extra information
-----------------
For more information, visit the official TACC documentation:
`<https://www.tacc.utexas.edu/user-services/user-guides/>`_


Now we should request a Node to work on. You can do this by 

