# Krita and Stable Diffusion aka AI Image Generation for "Otto-normalverbraucher"

---

## Check-in question

What kind of image processing software are YOU using?

---

## What is Stable Diffusion?

Everyone knows Stable Diffusion indirectly.

Whenever you generate images using a text prompt, a Stable Diffusion Algorithm is being used.

![bing ai](bing.png)

https://poloclub.github.io/diffusion-explainer/

... but this is not a presentation about Stable Diffusion.

---

## Concerns with online image generation

* You can only control the text prompt
* No control for: AI Model, training, resolution, etc.
* Concerns about privacy, training-data, etc.

---

## Comfy UI makes life easier

Allows you to control the image generation with Stable Diffusion more precisely:

* Select Base Model
* Select Input data
* Allows for Text2Img, Img2Img...

---

# DEMO Comfy UI

http://10.23.23.2:8188

---

## But still...

... it's not really usable for digital artists.

---

## Krita Stable Diffusion Plugin to the rescue!

* Stable Diffusion directly integrated a image editor

https://github.com/Acly/krita-ai-diffusion

---

## What's Krita?

* Adobe Photoshop inspired
* Open Source

---

## Features

* Very easy installation
* Works Out-of-the-box:
  * Installs Comfy UI with everything included
  * Works with CPU or GPU (or GPUaaS)

Requirements for local generation:

* NVidia GPU, at least 8GB VRam (depending on BaseModel)

There is a CPU fallback, but takes 10x longer to render

---

## Installation

Take this link:

`https://github.com/Acly/krita-ai-diffusion/releases/download/v1.17.1/krita_ai_diffusion-1.17.1.zip`

And paste it into Krita:

![install](install.png)

---

## Enable Plugin

1. Restart Krita
2. Enable Plugin

![enable](enable.png)

---

## Add AI Generation Docket

![docket](docket.png)

---

## Inpainting DEMO: Image generation / composition with (negative) prompts

* Example prompt: `Summer beach, palms, sunset, lens flare`
* Negative prompt: `people, clouds`

Add a sand castle to the image.

![beach](beach.png)

---

## Image references DEMO: With MY face

Add your face on generated images.

![kt](kt_source.png)

* Face reference
* Prompt: portrait, necktie, smiling, hands on chin

![ktresult](kt_result.png)

---

## Outpainting DEMO

Enlarge a picture (Iguazu Falls)

* Text prompt: `waterfalls, jungle, sky, clouds`

![landscape](landscape.png)

![landscape2](landscape-out.png)

---

## Digital Artwork DEMO: A fantasy oktoberfest

* Text prompt: `rabbit with beer in hand, oktoberfest`

Change some things in picture

---

## Digital Artwork DEMO: Poses

* Text prompt: `jumping princess, crown`

---

## Upscaling DEMO: Navy-CIS "Computer Enhance"

Usually used to upscale generated images to a higher resolution.

![low](low_res.png)

![high](upscaled.png)

---

## Some glossary

* Model Checkpoint: Trained Stable Diffusion Base Model

Checkpoint Models are trained to output specific styles (usually: 4-10 GB)

* LoRA: Low Rank Adaptations

Adapt a Checkpoint Model with additional data (usually 50MB - 200 MB)

* VAE: Variable Auto Encoder

Already part of Model Checkpoint. Controls Color and Sharpness of the output image.
You might want to use a custom VAE

![vae](VAE.png)

---

## In-Depth Topic: Krita Diffusion Plugin settings

---

## In-Depth Topic: Stable Diffusion Models

I want to use a specific Stable Diffusion Model!

Train them yourself or get them from

https://civitai.com/models

![civitai](civitai.png)

---

## My Setup & Questions

* CPU: AMD Ryzen 7900X
* GPU: NVidia
* Tablet: iPad Air 2020 w/ Apple Pencil
* Connected using Weylus 