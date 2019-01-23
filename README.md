## Performance Analysis of Vision Kernels on Embedded CPU, GPU and FPGA:
This repository contains benchmarking data and source code for evaluating the performance of 50+ vision kernels on embedded CPU, GPU and FPGA.
 
```
Note: The content of this repository is still under updating.
```

## Getting Started

Installation

* clone this repository with Xilinx's [PYNQ-ComputerVision](https://github.com/Xilinx/PYNQ-ComputerVision.git) submodules

```
git clone --recursive https://github.com/ISU-RCL/cvBench.git
```

## Vision Kernels

 
| Input Processing | Image Arithmatic | Filters       |  Image Analysis | Geometric Transforms|  Features  | Flow and Depts|
| -------------    | -------------    | ------------- | -------------   |    -------------    | ---------- | ----------    |
| combine          | AbsDiff          |  filter2D     | histogram       | affine warp         | canny      | OF pyramid    |
| extract          | accumulate       |  sobel        |histogram equalization|perspective warp| fast       | stereoBM      | 
| color convert    |accumulate squared|  box filter   |integral image   | scaling             | harris     |               |
| bitdepth convert |accumulate weighted| dilate       |mean std dev     | remap               |            |               | 
| table lookup     | add/subtract     |  erode        |min/max loc      |                     |            |               | 
|                  |  mulitply        |  median       |                 |                     |            |               | 
|                  | threshold        | pyramidUp     |                 |                     |            |               | 
|             | bitwise and,or,xor,not| pyramidDown   |                 |                     |            |               | 
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
The source for this project is licensed under the 3-Clause BSD License
