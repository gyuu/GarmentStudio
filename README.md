# GarmentStudio

## 环境搭建

使用 QT 5.7, MinGW 版本。

### freeglut

下载 http://www.transmissionzero.co.uk/computing/using-glut-with-mingw/ 提供的 freeglut 包。

解压得到 bin，lib，include。

1. 把 include 中的 GL 文件夹 放到 Delfem 库的 include 中。
2. 将 lib 下的两个 .a 文件拷贝到 DelFEM\lib 目录下。
3. 把 freeglut.dll 的 32 位版本拷到项目根目录下。

### 使用 QT 自带的 mingw32-make 进行编译即可。

## ORIGINAL README

================================================
SOURCE README FOR SENSITIVE COUTURE
Nobuyuki Umetani (umetani@ui.is.s.u-tokyo.ac.jp)
================================================


REFERENCES
==========
This code is the implementation of the following paper. Note that implementation may not be exact. Please cite this paper if you use our implementation.

N.Umetani, D.Kaufman, T.Igarashi, E.Grinspun, "Sensitive Couture for Interactive Garment Editing and Modeling", Transaction of ACM SIGGRAPH, Vol. 30, No. 4, 2011



Required 
========
We have been running our demo using Core 2 Duo 2.66 GHz 64bit machine with 4Gb RAM. We use OpenGL in the program, so graphical hardware is necessary.


Compiling
=========
The command "make" should compile and link the program.


The Design Window
===================

Tools
-----
To change the tool, press right button and select tool from pop-up menu.
+ Drag : you can drag vertex/edge/loop of a pattern.
+ Dart Cutter : you can draw dart on a pattern. 
+ Edit Curve : you can grab the curve by click and dragging a polyline edge.
+ ChangeToLine : you can change a polyline edge to line.
+ ChangeToPolyline : you can change a line edge to a polyline edge.
+ SmoothPolyline : you can smooth a polyline edge by moving mouse with left button pressed near the polyline edge.

Keyboard
------
+ ' '  : change 3D model
+ 'b'  : Initialize the simulation 

View Change
-----------
This design window should be activated so as to change the view of the design window.
+ Pan : Shift+Left drag
+ Zoom : Page Up / Down



The Simulation Window
=====================

Texture
-------
you can change texture of cloth from pop up menu. select [texture] and chose one from submenu.

View Change
------
This design window should be activated so as to change the view of the simulation window.
+ Pan : Shift+Left drag
+ Rotataion : Ctrl+Left drag



