# withcode
Offline python module to match visualisation and sound features of create.withcode.uk

## Purpose
Create.withcode.uk is designed for teachers and students to write, run, debug and share code on almost any device. 
It has a module designed to make it simple for students to explore how bitmap images can be displayed from pixel data

For example, you can use https://tools.withcode.uk/bitmap/ to generate the pixel data and python code for any image like this: https://create.withcode.uk/python/GWg

![image](https://user-images.githubusercontent.com/760604/154808133-9335c00c-6c19-4a21-8bb4-da0a145d5aea.png)

This module is designed to allow the same functionality as create.withcode.uk's withcode module with real 'offline' python

## Usage
import the withcode module to be able to quickly display 2d lists as a bitmap image:
  
```
# visualise black and white data as an image
data = [[0, 1, 0, 1],
        [1, 0, 1, 0],
        [0, 1, 0, 1],
        [1, 0, 1, 0]]

import withcode
i = withcode.Image()
i.draw(data)
```
Try this online: https://create.withcode.uk/python/GWi

Images can be:
- black and white if the 2d list contains 0 for black and 1 for black for each pixel. Example: https://create.withcode.uk/python/GWi
- greyscale if the 2d list contains numbers between 0-255 for each pixel where 0 is black and 255 is white. Example: https://create.withcode.uk/python/GWj
- RGB colour if the pixel data is a 3d list (a 2d list where each pixel is a list of red, green and blue values between 0 and 255): Example: https://create.withcode.uk/python/GWk

## Install
If you want to run code that uses the withcode module offline in python without using create.withcode.uk then you can install it via the following command:
```
pip install withcode
```

If you use Thonny, you do this by clicking on the `Tools` menu then select `Manage Packages` and search for the withcode module
