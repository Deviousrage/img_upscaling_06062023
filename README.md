# gan_training.ipynb 2024-01-03
Image upscaling to higher resolution, test for GAN scheme  
inspired by:  https://arxiv.org/abs/1609.04802  
This repository does not contain trained weights or training data  

## Some settings
  Generator with 22 blocks of layers and 1,697,155 trainable parameters, full convolutional  
loss: mse(x) + log(discriminator(x))  
  Discriminator with 9 blocks of layers and 5,215,425 trainable parameters, full convolutional  
loss: log(discriminator(y)) + log(1-discriminator(generator(x)))  

optimizers.Adam(1e-4,beta_1=0.9)

## Notes
Currently all training images stored on my local hard drive and calculation made with specific environment for utilization GPU. So i can't guarantee it will run anywhere else

## Results

input:  
![input](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/5ca6b030-1ac4-4348-822e-60519eb8c154)  

30 epochs: 
![generated_output_2024-01-02_12-52-10](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/288e032d-f9cd-45a8-ae5b-9650328e5e70) 


50 epochs: 
![generated_output_2024-01-03_12-48-07](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/e37ac9cf-fc0e-4530-b6b1-c97f9055d4f4) 


## TODO: 
write environment specification

