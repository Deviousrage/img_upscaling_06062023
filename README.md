# gan_training.ipynb 2024-01-03
Image upscaling to higher resolution, test for GAN scheme  
inspired by:  https://arxiv.org/abs/1609.04802  
This repository does not contain trained weights or training data  

## Some settings
  Generator with 1549443 trainable parameters, full convolutional  
loss: mse(x) + log(discriminator(x))  
  Discriminator with 5,215,425 trainable parameters, full convolutional  
loss: log(discriminator(y)) + log(1-discriminator(generator(x)))  

optimizers.Adam(1e-4,beta_1=0.9)

## Notes
Currently all training images stored on my local hard drive and calculation made with specific environment for utilization GPU. So i can't guarantee it will run anywhere else

## Results

input:  
![input_stretched](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/34cd5223-24df-4359-b855-a9306cd84e57) 


50 epochs: 

![generated_output_2024-01-09_10-10-22](https://github.com/Deviousrage/img_upscaling_06062023/assets/124791262/05ab7391-0e30-4048-8d0c-d2c25dedcd1f)


## TODO: 
write environment specification

