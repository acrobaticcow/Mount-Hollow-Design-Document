## Fragment shader

Is a code that run for every pixel in a area and change its colors. 

We need to know the location of the pixel before any calculation can happen. To do this we use the UV coordinate.

It important to remember that each pixel **contains 3 channels** that display The 3 Primary Colors: red, green and blue. 
### UV Coordinate

A UV is a vector range from 0 -> 1 no matter the resolution or shape. 

It also use to visually represent the color channels of a pixel. A top left (0,1) is green, the bottom-left is (1,0), and the middle is yellow (1,1) `because yellow is the combination of red and green`. 

The UV is use to provide the address for the texture to put in. We can offset or distort the address to create cool effect 😎

## Godot usage

### Getting started

First, declare the type of shader: 

```c++
shader_type canvas_item;
```

We declare the fragment function which is a piece of code that will be execute on every pixels

```c++
void fragment () {}
```


### UV basics

