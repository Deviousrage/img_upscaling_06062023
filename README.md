# img_upscaling_06062023
Image upscaling to higher resolution, test for GAN scheme
This repository does not contain trained weights and training data

  notebooka76d346fe3.ipynb  
The content of the notebook I found at the beginning doesn't make much sense. At least looks like it used target training image in the prediction output. I got rid of it and here is the result

  08062023_modified_version.ipynb  
Next one. Here I used a scheme submitted in the paper https://arxiv.org/abs/1609.04802 . Adjusted some numbers, but in the end it didn't work. Launch cause kernel death. In most cases it mean that memory overflows, but lack of setting's abilities and mostly auto corrections in layers, I can't easily approve it
