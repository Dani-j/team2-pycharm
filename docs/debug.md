---
layout: default
title: Debugging Application
nav_order: 4
---

# Debug your Python application
{: .no_toc }
In this procedure, you will debug your first python application. To eliminate any potential bugs, programmers usually use debugging tools to find bugs in their project. By the end of this procedure, you will be able to debug your Python application.

## Pre-requisites
Before debugging, make sure you have met the following requirements:
* You have installed the Python downloaded from [https://www.python.org](https://www.python.org).
* You have opened an existing project or created a new project.

## Instructions
1. The following is a piece of code for demonstration, and you want to use it to calculate the sum from one to five. However, there is a bug in it, so you get an output of 10 instead of 15.

    ![Sample Code](../../assets/images/docs/debug/foo.png "Sample Code")

2. To find out what is going wrong, you have to set a breakpoint. To create breakpoints, just click the line number in the gutter.

    ![Set Breakpoint](../../assets/images/docs/debug/breakpoint.png "Set Breakpoint")

3. Next, click the ![Run](../../assets/images/docs/debug/run.png "Run") icon in the gutter. It is near the ```main``` function.

    ![Run from gutter](../../assets/images/docs/debug/run_from_gutter.png "Run from gutter")

4. Pycharm will start a debugging session, and you can see the ```Frames``` and the ```Variables``` in the Debug tool window.

    ![Run from gutter](../../assets/images/docs/debug/debug_tool.png "Run from gutter")

5. Click the step over icon in the Debug tool window to see what your code does line by line. Therefore, you need not to set a breakpoint for each line.

    ![Step Over](../../assets/images/docs/debug/step_over.png "Run")

6. From the ```variable``` window, you will notice that the application only calculate the sum from one to four.

    ![Step Over](../../assets/images/docs/debug/sum.png "Run")

7. At last, you modify the code using ```for number in range(1, 6)``` instead of ```for number in range(1, 5)```, and then you get the right output ```15```.

    ![Step Over](../../assets/images/docs/debug/fixed.png "Run")