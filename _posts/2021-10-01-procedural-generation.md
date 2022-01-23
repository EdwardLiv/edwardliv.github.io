---
layout: post
title: "3D Procedural Terrain Generation"
subtitle: "Creating an Earth-like world in C++ OpenFrameworks"
background: '/img/posts/procedural-generation/hills.jpg'
---

I made a C++ [OpenFrameworks](https://openframeworks.cc/) application that can generate an endless amount of terrain [meshes](https://en.wikipedia.org/wiki/Polygon_mesh). The user can tweak parameters from the UI and get real-time updates. See the video below.

<iframe src="https://www.youtube.com/embed/L4ozXb8_jkY" height="500px" width="100%"></iframe>

[Procedural generation](https://en.wikipedia.org/wiki/Procedural_generation) is a method of creating data automatically, thus reducing development time significantly. It can be used for generating large virtual worlds. Minecraft and Civilization are popular video games that make use of this technique.

In order to create terrain with variable elevation, one would either have to manually draw the [heightmap](https://en.wikipedia.org/wiki/Heightmap), or use a noise function for outputting the height values. One such example is [simplex noise](https://en.wikipedia.org/wiki/Simplex_noise):

<style>
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
</style>

<img src="/img/posts/procedural-generation/noise.png" alt="Simplex noise" style="width:33%;height:33%;" class="center"/>

Multiple noise functions with different amplitude and frequency can be overlapped in order to simulate the larger and smaller features of a terrain, thus having a more natural look. I recommend reading [this glossary](http://libnoise.sourceforge.net/glossary/) to understand how it works.

The height values are also used as thresholds for separating biomes: mountains, hills, plains, coastlines, oceans. Terrain below a certain threshold is flattened for water effect. Each polygon is colored depending on the height of its vertices.

Seeds can be used for generating completely different maps, here are a few examples:

<img src="/img/posts/procedural-generation/grid.png" alt="Procedural generation" />

We can also tweak the color palette for either more vibrant or desaturated visuals, or maybe for a desert or glacial theme:

<img src="/img/posts/procedural-generation/color.png" alt="Procedural generation" />

Source code is [here](https://github.com/EdwardLiv/Procedural-Terrain-Generation).