# Take home submission - TX

This is an image-to-image latent diffusion model interface, which uses fixed CLIP tokenizer and pre-trained text encoder (CLIP ViT-L/14 by default).  

You can choose one of the following models for generation: 

```
['runwayml/stable-diffusion-v1-5',
'stabilityai/stable-diffusion-2',
'stabilityai/stable-diffusion-2-1',
'CompVis/stable-diffusion-v1-4'].
```

The design choice is made based on [the HuggingFace image-to-image pipeline](https://github.com/huggingface/diffusers/blob/v0.20.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py), except that the code here is simpler with more comments.


You can see the generated images and evaluation outputs in [this colab notebook](https://colab.research.google.com/drive/1kHNcq9gvpz0TrazPyybSNibcHP_JKkTg?usp=sharing).
The code for the ImageToImageDiffuser class in this notebook is a little bit different because it's adapted to torch.nn.module with a foward function so I can run the Meta flop counter.  Please see the .py file as my submission. 









