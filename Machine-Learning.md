Machine learning CheatSheet
----------------------------------

This contains many classical equations and diagrams on machine learning, which will help you quickly recall knowledge and ideas on machine learning.

The cheat sheet will also appeal to someone who is preparing for a job interview related to machine learning.

Download PDF
--------------------------
https://github.com/soulmachine/machine-learning-cheat-sheet/blob/master/machine-learning-cheat-sheet.pdf

How to compile
--------------------------
docker pull soulmachine/texlive
docker run -it --rm -v $(pwd):/data -w /data soulmachine/texlive xelatex -synctex=1 --enable-write18 -interaction=nonstopmode machine-learning-cheat-sheet.tex
LaTeX template
This open-source book adopts the Springer latex template.

How to compile on Windows
------------------------------------
Install Tex Live 2014, then add its bin path for example D:\texlive\2012\bin\win32 to he PATH environment variable.

Install TeXstudio.

Configure TeXstudio.
Run TeXstudio, click Options-->Configure Texstudio-->Commands, set XeLaTex to xelatex -synctex=1 -interaction=nonstopmode %.tex.

Click Options-->Configure Texstudio-->Build,
set Build & View to Compile & View,
set Default Compiler to XeLaTex,
set PDF Viewer to Internal PDF Viewer(windowed), so that when previewing it will pop up a standalone window, which will be convenient.

Compile. Use Open machine-learning-cheat-sheet.tex with TeXstudio，click the green arrow on the menu bar, then it will start to compile.
In the messages window below we can see the compilation command that TeXstudio is using is xelatex -synctex=1 --enable-write18 -interaction=nonstopmode "machine-learning-cheat-sheet".tex
