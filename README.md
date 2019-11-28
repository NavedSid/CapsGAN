# CapsGAN

Implementation of CapsGAN based on [Raeid Saqur et al](https://arxiv.org/pdf/1806.03968.pdf) paper.

The purpose of the repository is to be able to generate high quality faces. The dataset used for the purpose is [fhhq dataset](https://github.com/NVlabs/ffhq-dataset
). The model was trained on 128x128 thumbnail images.

The model was trained on 56k training images for 160 epochs (1 epoch is 1 pass over the entire train dataset).

Evaluation is based on the FID score. For baseline model DCGAN was used. A DCGAN trained for the same time provides FID score of 72.34 
while the CapsGAN provides a much better FID score at 31.25. The FID score was calculated on 50k test images.

# Result
DCGAN:
![](https://github.com/NavedSid/CapsGAN/blob/master/DCGAN/DCGANResult.png "DCGAN Result")

CapsGAN:
![](https://github.com/NavedSid/CapsGAN/blob/master/CapsGAN/CapsGANResult.png "CapsGAN Result")