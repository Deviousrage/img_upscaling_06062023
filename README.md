# img_upscaling_06062023,27112023
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

output 50 epochs: 
![Prince_result_2023-11-23_10-17-35](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/5c775d82-e277-41eb-b234-ec59fea54dfd)  

output 300 epochs:  
![Prince_result_2023-11-26_10-56-46](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/f740207a-c0f5-4b2b-a502-2749e22ab73b)  

## TODO: 
write environment specification

