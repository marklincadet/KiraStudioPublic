# Troubleshooting

This page will contain solutions and workaround to various common issues users have encountered. If you encounter other problems, please bring them to our attention in our Discord.

## Gray screen, misaligned or corrupted graphics (Windows)

Some older graphics cards have very poor OpenGL support on Windows. Here are a few examples reported by our users:

- Intel HD Graphics 3000 and 4000
- Nvidia GTX 1050
- AMD Radeon HD 7500 series

The first step should always be to **update your graphics drivers**. 

If that does not work, switching to a custom OpenGL renderer has been known to work for many people:

1. Download [Mesa3D](https://fdossena.com/?p=mesa/index.frag) for Windows 64-bit
2. Grab `opengl32.dll` from the downloaded zip
3. Put it in the same folder as `KiraStudio.exe`

Note that this may significantly reduce graphics performance inside the app if Mesa runs in software mode.