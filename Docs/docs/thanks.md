# Acknowledgements

KiraStudio uses the work of amazing developers and artists. This page attempts to acknowledge these contributions. 

## Licenses

The app uses a few library with permissive licenses, please go and support each of these projects.

### GLFW

[GLFW](https://www.glfw.org/) is a fantastic little window system for OpenGL and Vulkan apps. It is released under the zlib/libpng license, you will find the required text below which is taken from their [license page](https://www.glfw.org/license).

```text
Copyright © 2002-2006 Marcus Geelnard

Copyright © 2006-2019 Camilla Löwy

This software is provided ‘as-is’, without any express or implied warranty. In no event will the authors be held liable for any damages arising from the use of this software.

Permission is granted to anyone to use this software for any purpose, including commercial applications, and to alter it and redistribute it freely, subject to the following restrictions:

The origin of this software must not be misrepresented; you must not claim that you wrote the original software. If you use this software in a product, an acknowledgment in the product documentation would be appreciated but is not required.

Altered source versions must be plainly marked as such, and must not be misrepresented as being the original software.

This notice may not be removed or altered from any source distribution.
```

### YMFM

[YMFM](https://github.com/aaronsgiles/ymfm) is a great library for emulating many of the Yamaha sound chips. It is used in MAME and countless other projects. It is released under the BSD 3-Clause License.

```text
BSD 3-Clause License

Copyright (c) 2021, Aaron Giles
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### OGG/Vorbis

The [Vorbis](https://xiph.org/vorbis/) audio compression format and its OGG container format requires no introduction. The app uses it for both import and export. It is released under the BSD-3-Clause license.

```text
Copyright (c) 2002-2020 Xiph.org Foundation

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions
are met:

- Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.

- Redistributions in binary form must reproduce the above copyright
notice, this list of conditions and the following disclaimer in the
documentation and/or other materials provided with the distribution.

- Neither the name of the Xiph.org Foundation nor the names of its
contributors may be used to endorse or promote products derived from
this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE FOUNDATION
OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### GeneralUser GS

[GeneralUser GS 2.0.2](https://schristiancollins.com/generaluser.php) by S. Christian Collins is amazingly compact GS/GM SoundFont. It punches way about its weight in kilobyes. Please go and support their work, or [buy them a coffee here](https://buymeacoffee.com/schristiancollins).

The app comes bundles with an OGG-compressed version of the SoundFont to keep the size of the app relatively small. The compressed version was made using MuseScore's amazing [sftools](https://github.com/musescore/sftools).

Im am including the license that comes with the SoundFont here for completeness.

```text
*** GeneralUser GS v2.0.1 ***
***      License v2.0     ***

** License of the complete work **
You may use GeneralUser GS without restriction for your own music creation,
private or commercial. This SoundFont bank is provided to the community free of
charge. Please feel free to use it in your software projects, and to modify the
SoundFont bank or its packaging to suit your needs.

** License of contained samples **
GeneralUser GS inherits the usage rights of the samples contained within, all of
which allow full use in music production, including the ability to make profit
from musical recordings created with GeneralUser GS.

Many of the samples are original, but some were taken from other banks freely
(and legally) available on the Internet from various SoundFont websites. Because
GeneralUser GS originated as a personal project with no intention for
publication, I cannot be 100% sure where all of the samples originated, although
I do know that none of them came from commercially published SoundFont packages
or sample CDs. Regardless, many "free" SoundFonts available on the web may
indeed contain samples of questionable origin. My understanding of the
copyrights of all samples is only as good as the information provided by the
original sources. If you become aware of any restricted samples being used in
GeneralUser GS, please let me know so I can replace them.

This uncertainty may concern you if you intend to use GeneralUser GS in a
commercial software product. That being said, I have never received any
complaint regarding sample ownership since I published the original GeneralUser
GS back in 2000, and as far as I am aware, neither have any of the companies
creating commercial software products using GeneralUser GS.

** More info **
If you plan to feature GeneralUser GS on your own website, please do not link
directly to my download files. Either link to my website, or provide your own
local copy instead.

I hope you enjoy GeneralUser GS! This SoundFont bank is the product of many
years of hard work.

You can find updates to GeneralUser GS and more of my virtual instruments at:
http://www.schristiancollins.com

I can be reached via the contact page on my website here:
https://www.schristiancollins.com/contact

Thank you!
-~Chris
```

## Other Projects

I want to acknowledge some other projects that, while not providing code or libraries directly, were either inspirations or useful tools during development.

### MeltySynth

[MeltySynth](https://github.com/sinshu/meltysynth) was the original code I first looked at when trying to implement SoundFont support years ago. While the app does not use any of its code, I do want to acknowledge and draw attention to this great little project as it was a huge inspiration.

### Polyphone

[Polyphone](https://www.polyphone.io/) is the de-facto tool for SoundFont editing. I used it as a benchmark to compared against during development. Not only is it a great tool, but the website as a ever growing collection of user-generated SoundFonts, which makes it a great resource for KiraStudio as well.

### FamiStudio

While KiraStudio is closed source at the moment, the code is an evolution of my other open-source project, [FamiStudio](http://famistudio.org). If you are curious how a slightly more primitive version of the app was put together, go check it out.

## Demo Songs

The app comes with a few demo songs. Most of them are covers, please go support both the original composers and the cover artists.

- Deltarune - Ruder Buster (by [Toby Fox](https://x.com/tobyfox), cover by [How2Bboss](https://www.youtube.com/@How2Bboss))
- The Legend of Zero Force (by [Zabutom](https://www.youtube.com/@zabutom), cover by [How2Bboss](https://www.youtube.com/@How2Bboss))
- Theme of Mega Man - Battle Network 6 (by Yoshino Aoki, cover by Omega Zero)

Some of these demo songs require external SoundFonts, please visit [this page](soundfonts.md) for direct download links.