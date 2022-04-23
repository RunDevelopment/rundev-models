# Wood

This directory contains models for upscaling wood textures.

## Models

### 4x-Wood-BC1

[Link](./4x-Wood-BC1.pth)

```
Name: 4x-Wood-BC1
Model Architecture: ESRGAN
Scale: 4
Purpose: A 4x upscaler for BC1-compressed wood textures.

Iteration: 100k
batch_size: 8
HR_size: 128
Epoch: 81
Dataset: Custom. See below.
Dataset_size: 180
Pretrained_Model_G: 4xESRGAN.pth
```

Description: A 4x upscaler for BC1-compressed wood textures. The model was trained on wood planks, wood stems, and a bit of tree bark. It performs reasonably well on woody textures and produces sharp outputs. However, it also tends to slightly shift the hue of the image, so results might appear slightly more red.


## Data sources

The model in this directory were trained on wood textures from the following sources:

- https://polyhaven.com/
- https://freepbr.com/
- https://ambientcg.com/
- https://texture.ninja/

The data was also augmented by randomly adjusting the hue and saturation of images.
