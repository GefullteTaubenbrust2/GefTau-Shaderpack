# GefTau Shaderpack for Minetest
This pack is intended to improve Minetest's visuals by modifying its shader code. The pack adds the following effects:
- Better Shadow/artificial Light Colors
- Color Grading
- Translucent Foliage
- Glossy water
- God Rays

The nice thing about Minetest shaders is that you can modify them easily without having to compile the rest of the game. However, this also means that they have to work with what the engine provides. There are certainly other effects or better ways of implementing the ones provided, but that would require changes to the game's source code, however small they may be.
# Installation
1. Download the provided files
2. Go to your Minetest folder
3. Go to `client/shaders`
5. Copy the shaderpack into that folder
6. Profit!

If you want to uninstall, either download the default shaders from [the Minetest repository](https://github.com/minetest/minetest) or create a backup of your current shaders and copy whichever you chose into the `client/shaders` folder.

# Performance
Of course there is at least some performance impact that comes with these effects. The god rays in particular are quite heavy on the graphics card. The same is somewhat true for the wavy water. If you should run into lag issues, both can be disabled:
1. Go to your `client/shaders` folder after installing or the master folder before installing
2. Open `nodes_shader/opengl_fragment.glsl` with a text editor of your choosing
3. Comment out one or more of the options `#define ENABLE_GOD_RAYS` and `#define ENABLE_FRAGMENT_WAVES` by writing `//` before them
4. Save changes

# Gallery
![screenshot_20231030_175105](https://github.com/GefullteTaubenbrust2/Minetest-Shaderpack/assets/72752000/9b42db6d-398e-44fb-8b2e-a698f6147ba2)
![screenshot_20231031_104621](https://github.com/GefullteTaubenbrust2/Minetest-Shaderpack/assets/72752000/455152bb-9ac3-42e4-9088-78e01264d59d)
![screenshot_20231031_104547](https://github.com/GefullteTaubenbrust2/Minetest-Shaderpack/assets/72752000/b088067f-476e-43dd-a459-bf952eb81574)
![screenshot_20231031_104433](https://github.com/GefullteTaubenbrust2/Minetest-Shaderpack/assets/72752000/84defa40-133e-4981-a76e-810dd8f8f4b8)
![screenshot_20231030_130006](https://github.com/GefullteTaubenbrust2/Minetest-Shaderpack/assets/72752000/b8c8663c-5d76-4287-bce2-83e89e94567e)
