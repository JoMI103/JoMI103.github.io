---
caption: #what displays in the portfolio grid:
  title: Voxel World
  subtitle: Voxel Procederal Generation
  thumbnail: assets/img/portfolio/Covers/Cover_VoxelWorld.png
  
#what displays when the item is clicked:
title: Voxel World
subtitle: 
#image: assets/img/portfolio/BewareTheSheep.png #main image, can be a link or a file in assets/img/portfolio
#alt: image alt text
videoLink: ""

---



<div align = "Left">
Concept: Voxel world is the ground up for my futere game: Robotorio, a voxel factory game inspired by Factorio, where you control a robot with the sole objective of collecting resources from a mine for its creator.    <br> <br> <br>
</div>

<div align = "Center"><b><h3> Current state</h3></b> </div>

<div class="Column">
    <img src="assets/img/portfolio/Robotorio/28fps.png" alt="img2" style="width:100%">
  </div>

<div align = "Left"> Right now, using a 1050 Ti, I'm rendering a world with 1280 by 1280 by 1280 voxels (2 bilion Voxels) at 28 FPS, likely with non-optimized vertex and fragment shaders, without simpler optimizations, such as skiping chunks outside camera frustrum or not rendering the three back-facing voxel faces, and without more advanced techniques for this context, such as occlusion culling and a LOD system. <br>
All of this was achieved using the OpenGL function glMultiDrawArraysIndirect, which Unity does not support. Therefore, I had to developed an external plugin.
<br><br>
</div>

<div class="Column">
  <div class="Column">
      <div align = "Center"><i> Terrain (Normals, Texture, light, light and shadows, Close up)
    <img src="assets/img/portfolio/Robotorio/Normals.png" alt="img2" style="width:100%">
   
 
  <div class="Column">
    <img src="assets/img/portfolio/Robotorio/Texture.png" alt="img2" style="width:100%">

  </div>
  <div class="Column">
    <img src="assets/img/portfolio/Robotorio/Light.png" alt="img2" style="width:100%">

  </div>
  <div class="Column">
    <img src="assets/img/portfolio/Robotorio/Shadow.png" alt="img2" style="width:100%">
  </div>
  <div class="Column">
  <img src="assets/img/portfolio/Robotorio/CloseRange.png" alt="img2" style="width:100%">

</div>

<div align = "Left"><br>I also created a system that converts .point files (from MagicaVoxel) into data compatible with the renderer. The system takes the voxel data, generates the external faces, and merges them using a greedy mesher algorithm. Additionally, the color data is transferred to a texture that the renderer uses. <br> <br> </div>

  <div class="Column">
  <img src="assets/img/portfolio/Robotorio/Robos.png" alt="img2" style="width:100%">
  </div>
  <div class="Column">
  <img src="assets/img/portfolio/Robotorio/tex.png" alt="img2" style="width:50%">
  </div>
  
   <div class="Column">
  <img src="assets/img/portfolio/Robotorio/RobosTerreno.png" alt="img2" style="width:100%">
  </div>
  
  <div align = "Left"> As you can see in the last image, this enables the use of other blocks to texture the terrain<br> <br> </div>
  
  <div align = "Left"> This was a pretty complex project, especially when dealing with the plugin development in unity, which was buggy and lacked proper documentation.<br> <br> </div>