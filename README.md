# CS330 Final Project - 3D Scene Renderer

## Overview
This project is a 3D scene renderer created by Brad Mills for CS330. It uses OpenGL to render a scene containing multiple objects including a table, book, soap bar, cologne bottle with cap, and two cylinders. The scene includes lighting effects, texture mapping, and camera controls.

## Features
- **Interactive Camera**: Move around the scene using WASD keys, Q/E for up/down, and mouse for rotation
- **Projection Switching**: Toggle between perspective and orthographic views with 'P' key
- **Dynamic Lighting**: Two point lights with attenuation effects
- **Texture Mapping**: Multiple textures applied to different objects
- **Mouse Controls**: Sensitivity adjustment via scroll wheel
- **Objects**:
  - Table top with marble texture
  - Book with cover texture
  - Soap bar
  - Cologne bottle with cap
  - Two cylinders

## Dependencies
- GLFW: Window and input management
- GLEW: OpenGL extension loading
- GLM: Math operations for transformations
- STB_IMAGE: Texture loading
- Custom Cylinder class (Dependencies/cylinder/Cylinder.h)

## Prerequisites
- C++ compiler supporting C++11 or later
- OpenGL 4.4 or higher
- Required libraries installed (GLFW, GLEW, GLM, STB_IMAGE)

## Building and Running
1. Ensure all dependencies are installed and properly linked
2. Place texture files in `Resources/Textures/` directory:
   - table.jfif (marble texture)
   - book.png
   - soap.png
   - dust.jpg
3. Compile the source code with your preferred C++ compiler
4. Run the executable

## Controls
- **WASD**: Move camera forward/back/left/right
- **Q/E**: Move camera up/down
- **Mouse**: Look around (click and drag)
- **Scroll Wheel**: Adjust movement speed
- **P**: Toggle between perspective and orthographic projection
- **ESC**: Close the application

## Project Structure
- **Main File**: Contains the main rendering loop and initialization
- **Shader Programs**: Vertex and fragment shaders for lighting and texture handling
- **Mesh Data**: Vertex data for all objects stored in UCreateMesh()
- **Textures**: Loaded from Resources/Textures directory

## Technical Details
- **OpenGL Version**: 4.4 Core Profile
- **Window Size**: 800x600 pixels
- **Lighting**: Phong lighting model with two point lights
- **Coordinate System**: Right-handed
- **Texture Units**: Uses 5 texture units (0-4)

## Known Issues
- Mouse callback is implemented but commented out in the main loop
- Texture loading paths are relative and may need adjustment
- Limited error handling for shader compilation failures

## Credits
- Created by: Brad Mills
- Course: CS330
- Libraries: GLFW, GLEW, GLM, STB_IMAGE

For any questions or issues, please contact the author.
