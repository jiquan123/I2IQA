# I2IQA
This is the official repo of the paper [PKU-I2IQA: An Image-to-Image Quality
 Assessment Database for AI Generated Images](http://arxiv.org/abs/2311.15556):
  ```
@misc{yuan2023pkui2iqa,
      title={PKU-I2IQA: An Image-to-Image Quality Assessment Database for AI Generated Images}, 
      author={Jiquan Yuan and Xinyan Cao and Changjin Li and Fanyi Yang and Jinlong Lin and Xixin Cao},
      year={2023},
      eprint={2311.15556},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
<hr />

> **Abstract:** *As image generation technology advances, AI-based image generation has been applied in various fields and Artificial Intelligence Generated Content (AIGC) has garnered widespread attention. However, the development of AI-based image generative models also brings new problems and challenges. A significant challenge is that AI-generated images (AIGI) may exhibit unique distortions compared to natural images, and not all generated images meet the requirements of the real world. Therefore, it is of great significance to evaluate AIGIs more comprehensively. Although previous work has established several human perception-based AIGC image quality assessment (AIGCIQA) databases for text-generated images, the AI image generation technology includes scenarios like text-to-image and image-to-image, and assessing only the images generated by text-to-image models is insufficient. To address this issue, we establish a human perception-based image-to-image AIGCIQA database, named PKU-I2IQA. We conduct a well-organized subjective experiment to collect quality labels for AIGIs and then conduct a comprehensive analysis of the PKU-I2IQA database. Furthermore, we propose two benchmark models: NR-AIGCIQA based on the no-reference image quality assessment method and FR-AIGCIQA based on the full-reference image quality assessment method. Finally, leveraging this database, we conduct benchmark experiments and compare the performance of the proposed benchmark models.* 
<hr />

### Sampled images
Different scenes and styles of images sampled from the PKU-I2IQA
database, generated by Midjourney and Stable Diffusion V1.5.

![samples_imgs](https://github.com/jiquan123/I2IQA/blob/main/Pic/1.png)

### NR-AIGCIQA

![NR_imgs](https://github.com/jiquan123/I2IQA/blob/main/Pic/5.png)

### FR-AIGCIQA

![FR_imgs](https://github.com/jiquan123/I2IQA/blob/main/Pic/6.png)

### Pre-trained visual backbone
For feature extraction from input images, we selected several backbone
network models pre-trained on the ImageNet dataset, including:
-  VGG16 [weights](https://download.pytorch.org/models/vgg16-397923af.pth)
-  VGG19 [weights](https://download.pytorch.org/models/vgg19-dcbb9e9d.pth)
-  ResNet18 [weights](https://download.pytorch.org/models/resnet18-f37072fd.pth)
-  ResNet50 [weights](https://download.pytorch.org/models/resnet50-0676ba61.pth)
-  InceptionV4 [weights](http://data.lip6.fr/cadene/pretrainedmodels/inceptionv4-8e4777a0.pth)

### More experimental results
-  cross-model evaluation experiments

| Method | Quality | | | Authenticity | | | Correspondence | | | Final_score | |
|--------|--------|--------|--------|------------|--------|--------|---------------|--------|--------|-------------|--------|
|        | SRCC   | PLCC   | SRCC   | PLCC        | SRCC   | PLCC   | SRCC          | PLCC   | SRCC   | PLCC        | SRCC   |
| VGG16* | 0.1796 | 0.2046 | 0.1907 | 0.2039      | 0.2989 | 0.2849 | 0.2600        | 0.3013 | 0.2515 | 0.2740      | 0.2778 |
| VGG19* | 0.2237 | 0.2370 | 0.2766 | 0.2844      | 0.3629 | 0.3453 | 0.2241        | 0.2415 | 0.2934 | 0.2959      | 0.3213 |
| ResNet18* | 0.2388 | 0.2614 | 0.2731 | 0.2665 | 0.3504 | 0.3230 | 0.2891        | 0.2906 | 0.2626 | 0.2701      | 0.3006 |
| ResNet50* | 0.2110 | 0.2283 | 0.3033 | 0.2856 | 0.4177 | 0.3868 | 0.3158        | 0.3216 | 0.2297 | 0.2562      | 0.3117 |
| InceptionV4* | 0.2121 | 0.2162 | 0.2611 | 0.2788 | 0.3533 | 0.3559 | 0.2398    | 0.2599 | 0.2714 | 0.2632      | 0.3033 |
| VGG16 | 0.2515 | 0.2740 | 0.2778 | 0.2837 | 0.3793 | 0.3582 | 0.3052 | 0.3219 |
| VGG19 | 0.2934 | 0.2959 | 0.3213 | 0.3172 | 0.3599 | 0.3273 | 0.2913 | 0.3167 |
| ResNet18 | 0.2626 | 0.2701 | 0.3006 | 0.2937 | 0.4026 | 0.3703 | 0.2998 | 0.2993 |
| ResNet50 | 0.2297 | 0.2562 | 0.3117 | 0.3168 | 0.4277 | 0.3963 | 0.2963 | 0.3319 |
| InceptionV4 | 0.2714 | 0.2632 | 0.3033 | 0.2875 | 0.4122 | 0.3889 | 0.3076 | 0.3154 |


### Database
The constructed PKU-I2IQA database can be accessed using the links below.
Download PKU-I2IQA database:[[百度网盘](https://pan.baidu.com/s/1Jq6aAW5y3i_p5jgoRWvB8w ) 
(提取码：i2ia)].



### Contact
If you have any question, please contact yuanjiquan@stu.pku.edu.cn
