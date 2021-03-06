# Time domain signal plot
![](https://img.shields.io/badge/C++-95.6%-brightgreen.svg) ![](https://img.shields.io/badge/qt-5-yellow.svg)![](https://img.shields.io/badge/release-v2021.1.24-red.svg)

This project is about using the Qt platform to draw time-domain signal waveforms. It is worth noting that the dynamic waveforms are drawn here, that is, the multi-threading function in Qt is used.

## Software

In this project, the software and compilers we used are as follows：

- windows10
- Qt creator 4.9.0
- Qt 5.12.2
- Microsoft Visual C++ Complier 15.0(x86)

## Description 

The functions of each code file are described as follows(.h and .cpp)：

- **data_generate_thread**：thread function，continuous signal data is generated in this thread.
- **chartview**：mouse operation, including scroll wheel operation (screen zoom in or zoom out), mouse operation (screen zoom in, restore).
- **acousticwidget**：receiving time domain data and dynamic display operations, including the three operations of removing the beginning data, connecting the end data, and displaying the whole data.
- **mainwindow**：the function is directly associated with mainwindow.ui, call data_generate_thread, chartview, acousticwidget three functions to draw dynamic time-domain waveforms.
- **main**：call mainwindow function.

## Example

The running results of the project are as follows：

![img](https://github.com/blank1996/Signal_Plot/blob/main/gif_show.gif)



## change log

V1(2021.1.24)

- Upload code of project