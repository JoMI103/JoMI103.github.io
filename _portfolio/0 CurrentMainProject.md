---
caption: #what displays in the portfolio grid:
  title: Current Main Project
  subtitle: Voxel Factory Game
  thumbnail: assets/img/portfolio/Robotorio/CloseRange.png
  
#what displays when the item is clicked:
title: Voxel Factory Game
subtitle: 
#image: assets/img/portfolio/BewareTheSheep.png #main image, can be a link or a file in assets/img/portfolio
#alt: image alt text
videoLink: ""

---



<div align = "Left">
Concept: Robotorio (Temporary name) will be a voxel factory game inspired in Factorio, 
where you control a robot with the sole objective of colllecting resources from a mine for its creator. <br> <br> <br>
</div>

<div align = "Center"><b><h3> Current state</h3></b> </div>

<div class="Column">
    <img src="assets/img/portfolio/Robotorio/28fps.png" alt="img2" style="width:100%">
  </div>

<div align = "Center"> Right now, with a 1050 Ti, I'm rendering a world with 1280 by 1280 by 1280 voxels at 28 FPS with probably not optimized vertex and fragment shaders, without simpler optimizations like not dealing with chunks that are not in the camera frustum and not rendering the 3 opposite triangles of the voxels. And without more complex optimizations like occlusion culling and an LOD system. <br>
This was achieved with the OpenGL function glMultiDrawArraysIndirect, which Unity does not support. Therefore, I needed to create an external plugin (it was hell, because every time you test an external plugin, you need to restart Unity to update the plugin).
<br><br>
</div>

<div class="Column">
  <div class="Column">
      <div align = "Center"><i> Terrain (Normals, Texture, light, light and shadows, Close up)</b>
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

<div align = "Center"><br> Also i have made a system that converts .point files (created in MagicaVoxel) into data compatible with the renderer, the system takes the voxel data and generates the external faces and joins them with a greedy mesher algorithm, also the color data is transferred to a texture that the renderer uses. <br> <br> </div>

  <div class="Column">
  <img src="assets/img/portfolio/Robotorio/Robos.png" alt="img2" style="width:100%">
  </div>
  <div class="Column">
  <img src="assets/img/portfolio/Robotorio/tex.png" alt="img2" style="width:50%">
  </div>
  
   <div class="Column">
  <img src="assets/img/portfolio/Robotorio/RobosTerreno.png" alt="img2" style="width:100%">
  </div>
  
  <div align = "Center"><br> As you can see in the last image, this enables the use of other blocks to texture the terrain<br> <br> </div>