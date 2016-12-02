TODO - Add documentation

# Dev Setup #

- follow guide below for install glut
- hope everything works

how to guide copied from [https://www.cs.csustan.edu/~rsc/SDSU/GLUTinstall.html](https://www.cs.csustan.edu/~rsc/SDSU/GLUTinstall.html)


## Install GLUT ##
With thanks to Kamil Saykali of the EdCenter:
This part will show how to install the glut libraries and dll's (to download it go to http://reality.sgi.com/opengl/glut3/glut3.html )

1. After you have downloaded the glut.zip file (you should get the latest ver 3.7) unzip it into a folder
2. Inside the folder you should have:
  - `glut.dll`
  - `glut32.dll`
  - `glut.h`
  - `glut.lib`
  - `glut32.lib`
3. Copy both glut.dll and glut32.dll into your windows directory (windows or winnt, depends on if you are using Windows95/98 or Windows NT)
4. Copy your glut.h to:
  - `<drive>:\<VC++ path>\include\GL\glut.h`
  - *** put the drive where you installed VC++ instead of the <drive> ***
  - *** put the directory where you installed VC++ instead of the <VC++ path>
5. Copy your glut.lib and glut32.lib to:
  - `<drive>:\<VC++ path>\lib\glut.lib`
  - `<drive>:\<VC++ path>\lib\glut32.lib`
  - *** put the drive where you installed VC++ instead of the <drive> ***
  - *** put the directory where you installed VC++ instead of the <VC++ path>
6. That should be it for installed the glut libraries. The rest of this letter shows you how to setup VC++ so that you can use the glut libraries.
  -This will show you how to start up an opengl project and setup the setting so that you will be able to compile and run the program. This is assuming that you have already downloaded the appropriate files and installed them in the directories that there documentation tell you to. If you have not done that you need to do it before you can run or write an opengl program.
1. Start VC++ and create a new project.
2. The project has to be a "Win32 Console Application"
3. Type in the name of the project and where it will be on your hard drive.
4. Chose an empty project and click next or finish
5. First thing you need to do when the project opens up is to click on the "Project" menu item from the top.
6. Chose "Settings" (a window will come up)
7. On the left side of the window there are tabs, chose the "Link" tab
8. The string field labeled "Object/library modules" has a few lib files already set in it
9. Go to the end of this string field and enter:
  - `opengl32.lib glut32.lib glu32.lib`
10. Chose "OK" and that will include all the opengl libraries that you need
11. Now all you need to do is include <gl\glut.h> and you are ready to go
