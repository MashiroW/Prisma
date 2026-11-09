<div align="center">

<img src="docs/banner.png" alt="Prisma, faithful AI upscaling on your own PC" width="100%">

<br>

**Faithful AI upscaling, on your own PC.**

[![Version](https://img.shields.io/badge/version-1.2.0-2ea44f?style=for-the-badge)](https://github.com/MashiroW/Prisma/releases/latest) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDBoMTF2MTFIMHpNMTMgMGgxMXYxMUgxM3pNMCAxM2gxMXYxMUgwek0xMyAxM2gxMXYxMUgxM3oiLz48L3N2Zz4=&logoColor=white)](#requirements) [![NVIDIA](https://img.shields.io/badge/NVIDIA-4%20GB%2B-76B900?style=for-the-badge&logo=nvidia&logoColor=white)](#requirements) [![Licence](https://img.shields.io/badge/licence-non--commercial-8A5CF6?style=for-the-badge)](LICENSE.txt) [![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/MashiroW)

</div>

---

**Prisma** remakes your pictures in high definition: four times larger, sharper and cleaner, right on your own
computer. Nothing is uploaded, your pictures never leave your PC.

It shines on **video game assets** like sprites, textures, backgrounds and menus, and works just as well on
**any picture** you want to bring back to life.

<div align="center">
<img src="docs/ui/app.png" alt="Prisma's window with four pictures ready to be upscaled" width="100%">
</div>

## See it

<div align="center">

**Game art**

<img src="docs/examples/game.png" alt="A low-resolution game scene next to Prisma's 4x version, with a zoom" width="100%">

<br><br>

**Photos**

<img src="docs/examples/cat.png" alt="A low-resolution photo of a cat next to Prisma's 4x version, with a zoom" width="100%">

<br><br>

<img src="docs/examples/coffee.png" alt="A low-resolution photo of a coffee next to Prisma's 4x version, with a zoom" width="100%">

<sub>Left: the small picture given to Prisma. Right: Prisma's best model, 4×. The framed area is shown zoomed below.<br>
Example pictures by Kenney, Stefan van der Walt and Rachel Michetti, all in the public domain (CC0).</sub>

</div>

## How it works

Drop in your pictures, pick a model, press **Upscale**. Prisma does everything on your graphics card.

- **Whole folders at once.** Queue as many pictures as you like, stop any time and pick up where you left off.
- **A model for every picture.** Photos, anime, game textures or sprites: pick the one that fits.
- **Or a pipeline of your own.** Chain several models and picture steps, save them under a name, and use the result
  like any model. See [Pipelines](#pipelines) below.
- **Yours, locally.** No cloud, no account, no upload.

<div align="center">
<img src="docs/ui/models.png" alt="Prisma's model list, each model with its scale, licence and what it is best at" width="100%">
<br>
<sub>More than twenty models to choose from, for photos, anime, game textures and sprites, each with its own licence.</sub>
</div>

## Pipelines

Sometimes one model is not enough: a photo full of compression blocks is best cleaned first, then enlarged; a sprite
with transparency needs its edges handled with care. A **pipeline** is a series of steps you put together once and
reuse: models from the catalog, one after another, with picture steps around them.

<div align="center">
<img src="docs/ui/pipelines.png" alt="Prisma's Pipelines page: the list of pipelines on the left, the selected pipeline's steps on the right" width="100%">
</div>

1. Open the **Pipelines** page from the side bar.
2. Start from one of the examples (**Copy**) or a blank one (**New**), and give it a name.
3. Add the steps you need with **Add step**, put them in order with **Up** and **Down**, and pick each model step's
   model with **Model...**.
4. Press **Save**. Your pipeline now appears in the model list, under **Pipelines**, ready to be picked like a model.

The steps you can use:

| Step | What it does |
| :-- | :-- |
| **Model** | Any model of the catalog: enlarge, sharpen, denoise, clean up compression |
| **Border** and **Border taken off** | Add a margin around the picture before a model and remove it after, so the edges come out as clean as the middle |
| **Resize** | Bring the picture to a given scale, or to the final size, with the filter of your choice |
| **Enlarged pixel by pixel** | Double or triple the picture first without smoothing, handy for small pixel art |
| **Transparent pixels filled** | Fill the transparent areas from the nearest visible pixels, so no dark fringe appears around sprites |
| **Tones kept from the original** | Keep the original's colours and tones exactly, taking only the fine detail from the models |
| **Grey**, **Levels**, **One channel**, **Clip** | Simple adjustments, mostly for the transparency |

Pictures with transparency can get their own steps on the **Transparency steps** tab; otherwise their transparency
is simply resized with the picture. Prisma comes with a few example pipelines (a JPEG photo cleaned then enlarged, a
noisy photo denoised then enlarged, a faithful 4× in two passes, a 4× that keeps the original's colours, a fine 2×).
The same pipeline on the same picture always gives the same result.

## Download & install

1. Get the latest **`Prisma-x.y.z-win64.zip`** from the [**Releases**](../../releases) page.
2. Unzip it anywhere and run **`Prisma Setup.exe`**.
3. Accept the licence, then let Prisma set itself up.

The first run downloads Prisma's runtime and models from their official sources, each one checked before use.
After that, everything runs from your disk.

## Requirements

<div align="center">

| Component | Details |
| :-- | :-- |
| **System** | Windows 10 or 11, 64-bit |
| **Graphics card** | NVIDIA, **4 GB of VRAM** at least<br>8 GB for the best model |
| **Disk space** | About 12 GB, plus room for your pictures |
| **Internet** | Only once, for the first setup |

</div>

## Community

<div align="center">

Questions, tips, or something you made with Prisma to show off? Come and say hi.

[![Join the Discord](https://img.shields.io/badge/Discord-Join%20the%20server-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/9uprtBHsaJ)

</div>

## Licence

Prisma is **free for personal, non-commercial use**. See [`LICENSE.txt`](LICENSE.txt) for the details.
Prisma is closed source. It builds on open-source software and models, each credited with its own licence in
the licence folder that ships with the application.

Want to use Prisma in a **commercial or paid project**? Reach out on the
**[Discord](https://discord.gg/9uprtBHsaJ)** and we'll sort out a licence.

## Support

<div align="center">

If Prisma saves you time, you can support my work on **[GitHub Sponsors](https://github.com/sponsors/MashiroW)**.

[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/MashiroW)

</div>

<div align="center">
<br>
<img src="docs/icon.png" alt="Prisma" width="64">
<br>
<sub>Prisma, made by <strong>Mash</strong></sub>
</div>
