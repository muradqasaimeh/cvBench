## Benchmarking Analysis of Vision Kernels:
 
[![Latest Stable Version] 
[![Latest Stable Version](https://poser.pugx.org/phpunit/phpunit/version)](https://github.com/ISU-RCL/cvBench)


 [![Total Downloads](https://poser.pugx.org/phpunit/phpunit/downloads)](https://packagist.org/packages/phpunit/phpunit)
 [![License](https://poser.pugx.org/phpunit/phpunit/license)](https://packagist.org/packages/phpunit/phpunit)


* [Repository structure](#Repository_structure) 
* [ependencies and enviroment settings](#Dependencies_and_enviroment_settings)
* [Dependencies](#List of Vision Kernels)
* [Build](#build) 
* [References](#references)
* [License](#license) 


## Repository structure

This repository contains benchmarking data and source code for evaluating the performance of 50+ vision kernels on embedded CPU, GPU and FPGA.
  
This repository consists of two parts:
* FPGA testbenches:
* GPU testbenches:
    
## Dependencies and enviroment settings

Code Structure

## Getting Started

Installation

* clone this repository with Xilinx's [PYNQ-ComputerVision](https://github.com/Xilinx/PYNQ-ComputerVision.git) submodules

```
git clone --recursive https://github.com/ISU-RCL/cvBench.git
```

## List of Vision Kernels

 
| Input Processing | Image Arithmatic | Filters       |  Image Analysis | Geometric Transforms|  Features  | Flow and Depts|
| -------------    | -------------    | ------------- | -------------   |    -------------    | ---------- | ----------    |
| combine          | AbsDiff          |  filter2D     |calcHist         | affine warp         | canny      | OF pyramid    |
| extract          | accumulate       |  box filter   |equalizeHist     |perspective warp     | fast       | stereoBM      | 
| convertTo        |accumulate squared|  dilate   |integral image   | resize              | harris     |               |
| cvtConvert       |accumulate weighted| erode        |mean std dev     | remap               |            |               | 
| table lookup     | add/subtract     |  median       |min/max loc      |                     |            |               | 
|                  |  mulitply        | pyramidUp     |                 |                     |            |               | 
|                  | threshold        | pyramidDown   |                 |                     |            |               | 
|             | bitwise and,or,xor,not|               |                 |                     |            |               | 
|                  | magnitude        |               |                 |                     |            |               | 
|                  | phase            |               |                 |                     |            |               | 


### Hardware Environments
1. ARM-57 CPU
2. Nvidia's Jetson TX2 (Pascal GPU).
3. Xilinx's ZCU102 (FPGA).

### Software Environments
1. OpenCV 3.4
2. Nvidia's VisionWorks library.
3. Xilinx's xfOpenCV library.

## Running the tests
 
## Deployment
 


## License
The source for this project is licensed under the [3-Clause BSD License](LICENSE)
