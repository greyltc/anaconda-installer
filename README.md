# anaconda-installer
An installer that makes anaconda/python environments that I like

To create a win32 installer .exe that works on Windows XP run (in Anaconda 2.2) in this project folder:
```bash
conda update --all
conda install constructor
constructor --platform win-32 .
```
On Windows, start menu items will not be created. To get a bash terminal that that runs in the environment installed here run the following from a cmd.exe terminal:
```
set INSTALL_DIR=C:\python
%INSTALL_DIR%\pythonw.exe %INSTALL_DIR%\cwp.py %INSTALL_DIR% %INSTALL_DIR%\Library\bin\bash.exe --login -i --
```
where you edit `INSTALL_DIR` to be the directory that the user chose to install into when they ran the installer .exe on the target system.
