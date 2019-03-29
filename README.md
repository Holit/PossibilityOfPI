圆周率随机计算器（蒙特卡洛法）
=======
中文
* 编写及调试环境<br>
  Microsoft Visual Studio 2017 Community
* 基础运行(Debug)<br>
  Windows 10 Enterprise x64
-------
该计算器实现了使用蒙特卡洛法计算PI的值，程序设定时以将循环上限设置为100000000，即循环10亿次。
* 目的
使用C++实现蒙特卡洛算法
* 特性
  * 完成多次循环，从而模拟实验
  * 可变的上限，已注释的代码
* 原理
  * 程序建立数学模型，该数学模型描述如下：在平面直角坐标系内构造一个正方形，其四个顶点的坐标为(-1,1);(1,-1);(1,1);(-1,-1)。在该正方形中内嵌圆，选取正方形在第一象限中的部分。在该部分中取点，当点数足够多时可以近似计算其面积(~0.25)，每次取点时计算坐标是否满足 (x^2)+(y^2) <= 1 （即是否在圆内）。计算近似圆面积，从而得到PI。
  * 程序使用time作为随机数种子，获得在(0~1)中的两个随机数，模拟取点过程。
  

Peripheral random calculator (Monte Carlo method)
=======
English
* Writing and debugging environment<br>
  Microsoft Visual Studio 2017 Community
* Basic operation (Debug)<br>
  Windows 10 Enterprise x64
-------
The calculator implements the Monte Carlo method to calculate the value of PI, and the program is set to set the loop upper limit to 100000000, that is, 1 billion cycles.
* Purpose
Implementing Monte Carlo algorithm in C++
* Features
  * Complete multiple cycles to simulate the experiment
  * Variable upper limit, annotated code
* Principle
  * The program establishes a mathematical model, which is described as follows: Construct a square in a plane Cartesian coordinate system with coordinates of (-1,1); (1,-1); (1,1); -1, -1). A circle is embedded in the square, and a portion of the square in the first quadrant is selected. Take points in this part, when the number of points is enough, you can approximate the area (~0.25), and calculate whether the coordinates satisfy (x^2)+(y^2) <= 1 each time you take the point (ie whether it is inside the circle) ). Calculate the approximate circle area to get the PI.
  * The program uses time as a random number seed to obtain two random numbers in (0~1), simulating the point-taking process.
