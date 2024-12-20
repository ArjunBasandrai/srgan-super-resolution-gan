<h1 align="center">SRGAN Image Super Resolution</h1>

<p align="center">
  PyTorch implementation of <a href="https://arxiv.org/pdf/1609.04802">"Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial
Network"</a> trained on the <a href="https://www.kaggle.com/competitions/imagenet-object-localization-challenge/data">ImageNet 100K Subset</a> dataset
</p>

# Model Architecture

The model is built using the SRResNet and SRGAN architecture described in the paper

![image](https://github.com/user-attachments/assets/87cb4c15-e971-4fdf-b764-81047026fa29)

## Training Data

The model is trained on the <a href="https://www.kaggle.com/competitions/imagenet-object-localization-challenge/data">ImageNet 100K Subset</a> datatset available on Kaggle

## Super Resolution Results

Following are some of the results of the model on a few royalty free images from the internet

![image](https://github.com/user-attachments/assets/a9b0f4e3-cd07-4436-aba3-8b4a3e1de162)
![image](https://github.com/user-attachments/assets/29736d76-ca24-47fd-b302-9e7b049483f2)
![image](https://github.com/user-attachments/assets/50ce0e3f-b97a-47a9-a46e-0b4deea17bf6)
![image](https://github.com/user-attachments/assets/6b225244-009f-4cd4-98bd-56cb0cd8799e)
![image](https://github.com/user-attachments/assets/6876884e-c13a-4cf8-b638-704c213dfdf8)

Due to the hardware limitations, I was not able to train the models for the exact number of iterations described in the paper and I also had to take a subset of 30k images from the ImageNet dataset for the same reasons.

## Usage

1. Install dependencies
```bash
pip install torch torchvision matplotlib pillow numpy
```
2. Download the inference script located at `srgan-inference.ipynb`
3. Update the model path in the inference script, adjust image links as needed, and execute the cells.

## References

1. Ledig, C., Theis, L., Huszar, F., Caballero, J., Cunningham, A., Acosta, A., Aitken, A., Tejani, A., Totz, J., Wang, Z., & Shi, W. (2017). Photo-realistic single image super-resolution using a generative adversarial network. arXiv preprint arXiv:1609.04802. https://doi.org/10.48550/arXiv.1609.04802

2. Deng, J., Dong, W., Socher, R., Li, L.-J., Li, K., & Fei-Fei, L. (2009). ImageNet: A large-scale hierarchical image database. 2009 IEEE Conference on Computer Vision and Pattern Recognition, 248–255. https://doi.org/10.1109/CVPR.2009.5206848
