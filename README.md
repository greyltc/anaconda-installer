# anaconda-installer
An installer that makes anaconda/python environments that I like

To create a win32 installer .exe that works on Windows XP run (in Anaconda 2.2) in this project folder:
```bash
conda update --all
conda install constructor
constructor --platform win-32 .
```
