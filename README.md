# pyinstaller_bug

First clone the repo
Next, check that the executable works (it does nothing except import _sqlite3):

cd dist/pyinstaller_bug/
./pyinstaller_bug

Yay, nothing happens. Now, return to the top directory and move the mac compiled so file to the pyinstaller_bug directory:

cd ../../
mv _sqlite3.cpython-34m.so dist/pyinstaller_bug/

Return to the executable and run it:

cd dist/pyinstaller_bug/
./pyinstaller_bug

---------------------------------------------------------

ImportError: ~/bug_report/dist/pyinstaller_bug/_sqlite3.cpython-34m.so: invalid ELF header
pyinstaller_bug returned -1
