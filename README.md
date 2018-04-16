# Lambda School CS Wiki Repo

This is the Lambda School CS Wiki. Feel free to add things here that need to be written and shared but don't warrant their own repos.

Click [here](https://github.com/LambdaSchool/CS-Wiki/wiki) or the `Wiki` tab, above.


--------------------

Edit for _CS Lore > Getting Your C Compiler Installed > Windows > Option B: Cygwin_:

Change from:

Install Cygwin.
Launch a Windows command prompt.
Install the necessary packages by running the Cygwin Setup utility.
setup-x86_64.exe -q -P wget -P gcc-g++ -P make -P diffutils -P libmpfr-devel -P libgmp-devel -P libmpc-devel
Launch Cygwin-Terminal from its icon.

To something like:

Download and run either the Cygwin installer.
When you reach the “Select Packages” step (shown below), don’t bother selecting any packages yet. Click Next.
After the install completes, keep the installer. It is an executable named either `setup-x86.exe` or `setup-x86_64.exe`, and you’ll need it to add or remove Cygwin packages in the future. Moving the installer to the same folder where you installed Cygwin itself; typically `C:\cygwin` or `C:\cygwin64`.
Launch a Windows command prompt, and navigate to the directory where the Cygwin installer is currently located.
Run: `setup-x86_64.exe -q -P wget -P gcc-g++ -P make -P diffutils -P libmpfr-devel -P libgmp-devel -P libmpc-devel`. The initial command `setup-x86_64.exe` should be the name of the installer which you have moved to the Cygwin directory.
Once the install is complete, launch Cygwin-Terminal from its icon.
To compile the hello.c program: Inside of the Cygwin-Terminal, navigate to the directory which contains the source code, then enter: `gcc -Wall -Wextra -o hello hello.c`.
To run the program, now enter: `./hello`.

These instructions were paraphrased or quoted from http://preshing.com/20141108/how-to-install-the-latest-gcc-on-windows/
