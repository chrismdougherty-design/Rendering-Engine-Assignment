# Rendering Engine Assignment

# Rendering Engine Assignment – Lighting Techniques in Unreal Engine

## Group Members
- Chris Dougherty
- Clay Kelly
- Daniel Cabrera

## Course Information
**Course:** GDT-110-WF900A - Game Engine Architecture  
**Instructor:** Isac Artzi  
**Date:** 3/4/2026

## Project Overview
This project demonstrates **lighting techniques in Unreal Engine** and shows how lighting can improve visual quality while still being balanced with rendering performance. Our prototype scene was built to connect rendering theory to practical use inside a modern game engine.

The project includes:
- a basic 3D scene built in Unreal Engine
- multiple primitive objects arranged in the level
- imported assets and at least one applied texture
- lighting using a Directional Light and additional focused light sources
- performance testing using Unreal profiling tools
- optimization using **Level of Detail (LOD)**, **culling**, and **instancing**

Our goal was to show that lighting is not only a visual feature, but also part of a rendering workflow that must be optimized for better real-time performance.

## Rendering Topic
**Lighting Techniques in Unreal Engine**

### Research Question
How does Unreal Engine apply lighting techniques to improve visual quality while balancing rendering performance in a 3D game scene?

## Engine and Tools Used
- Unreal Engine 5.6.1
- GitHub Desktop
- GitHub

## How to Run the Project
1. Download or clone the repository from GitHub.
2. Open the project folder.
3. Locate the `.uproject` file.
4. Double-click the `.uproject` file to open the project in Unreal Engine 5.6.1.
5. If prompted to rebuild project files, allow Unreal Engine to continue.
6. Open the main level used for the assignment.
7. Press **Play** in the Unreal Editor to run the project.
8. Move through the scene and observe the lighting setup, textured objects, and optimization results.

## Project Features
- Uses at least five unique primitive objects or basic shapes
- Includes imported assets and textures
- Demonstrates lighting with a Directional Light and additional light sources
- Shows how lighting affects shadows, mood, visibility, and realism
- Uses profiling data to evaluate rendering performance
- Applies optimization methods including:
  - Level of Detail (LOD)
  - Culling
  - Instancing

## Performance Results
We created a baseline measurement table to compare performance before and after each optimization step.

| Metric | Baseline (Before) | After LOD | After Culling | After Instancing |
|--------|-------------------|-----------|---------------|------------------|
| FPS | 11 | 13 | 16 | 19 |
| Frame Time (ms) | 89 | 76 | 62 | 53 |
| Draw Calls | 420 | 210 | 160 | 105 |
| GPU Time (ms) | 83 | 73 | 61 | 50 |

## Summary of Results
After applying LOD, the scene showed a noticeable improvement in performance. FPS increased from 11 to 13, while frame time and GPU time decreased. This suggested that reducing model detail at a distance lowered rendering cost.

After applying culling, performance improved further because objects not visible to the camera no longer needed to be rendered. This reduced draw calls and helped increase FPS to 16.

After applying instancing, the project showed its best overall performance. Draw calls dropped significantly because repeated objects were rendered more efficiently. As a result, FPS increased to 19, while frame time and GPU time dropped to their lowest values.

These results show that LOD, culling, and instancing each improved performance, and together they made the scene render much more efficiently.

## References
Epic Games. (2026). *Introduction to performance profiling and configuration in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *Visibility and occlusion culling in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *Instanced Static Mesh Component in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *World Partition - Hierarchical Level of Detail in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *Viewport show flags in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *Using Distance Field Shadows in Unreal Engine*. Epic Games Documentation.  
Epic Games. (2026). *Guidelines for optimizing rendering for real-time in Unreal Engine*. Epic Games Documentation.
