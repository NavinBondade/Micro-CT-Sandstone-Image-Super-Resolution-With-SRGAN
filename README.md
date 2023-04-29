# Micro-CT Sandstone Super Image Super-Resolution With SRGAN
<p align="center">
<img src="https://d12oja0ew7x0i8.cloudfront.net/images/Article_Images/ImageForArticle_20456_16221026898502608.jpg">
</p>
<p>Sandstone is a clastic sedimentary rock composed mainly of sand-sized (0.0625 to 2 mm) silicate grains. It comprises about 20–25% of all sedimentary rocks. In this project, I have implemented and trained the Super Resolution GAN (SRGAN) deep learning model for performing image upscaling from the resolution of 64x64 to 256x256.</p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Sklearn</li>
</ul>
<h2>Dataset Visualization</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/data_2.png" width="550" height="600">
</p>
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/Data2.png" width="550" height="500">
</p>
<h2>What is Super Resolution GAN?</h2>
<p>Super-resolution GAN applies a deep network in combination with an adversary network to produce higher resolution images. During the training, A high-resolution image (HR) is downsampled to a low-resolution image (LR). A GAN generator upsamples LR images to super-resolution images (SR). We use a discriminator to distinguish the HR images and backpropagate the GAN loss to train the discriminator and the generator.</p>
<p>It uses a perceptual loss function which consists of an adversarial loss and a content loss. The adversarial loss pushes the solution to the natural image manifold using a discriminator network that is trained to differentiate between the super-resolved images and original photo-realistic images. In addition, the authors use a content loss motivated by perceptual similarity instead of similarity in pixel space.</p>
<p align="center">
<img src="https://camo.githubusercontent.com/7951c3e09e0a0db991436670150068e23293045fa700a858531a620037dfecae/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f323136342f312a43637145654a416136634f4250386137313359522d772e706e67" width="900" height="600">
</p>
<h2>Model Details</h2>
<p>The model has been trained on a sandstone micro-ct image dataset for 30 epochs. The dataset comprises downscaled images of sandstone with the shape of (64,64,3) and upscaled images of (256,256,3). The model used binary cross entropy and mean squared error as a loss function and Adam as the optimizer.</p>
<h2>Model Architecture</h2>   
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/SRGAN.png">
</p>
<h2>Model Training & Testing</h2>   
<p>The generator loss was 13.67 discriminator loss for fake images was 0.46 and for real images was 0.98.</p>
<h4>Generator Loss:</h4>   
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/Generator%20Loss.png" width="1000" height="350">
</p>
<h4>Discriminator Loss:</h4>  
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/Discriminator%20Loss.png" width="1000" height="350">
</p>
<h2>Model Prediction</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Micro-CT-Sandstone-Image-Super-Resolution-With-SRGAN/blob/main/Graphs/Output.png" width="800" height="1200">
</p>
<h2>Conclusion</h2>  
<p>In this project, I have implemented and trained SRGAN deep learning model for performing sandtone image upscaling from the resolution of 64x64 to 256x256.</p>  


