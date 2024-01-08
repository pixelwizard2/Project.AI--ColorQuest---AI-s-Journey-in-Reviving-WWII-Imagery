# Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery
_이미지 색상화를 위한 AI 기술 - 딥 러닝 아키텍처 비교 연구(GAN)_ <br>

<p align="right">
  <a href="https://blog.naver.com/pixelwizard/223315845279">
    <img src="https://img.shields.io/badge/한국어%20번역본-03C75A?style=flat-square&logo=Naver&logoColor=white" alt="네이버 블로그">
  </a> </p>  
  
​![2  arts_colorization](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/c8b0ad64-3e85-426a-836e-b4349d1f3b8a)

## Project Introduction (프로젝트 소개)

The aim of this project was to restore color to black and white photographs using deep learning technology. Various model architectures such as **CNN, Deep CNN, Autoencoder, and U-Net** were explored, and the potential for image generation using **GAN (Generative Adversarial Networks)** was tested. <br> 



<pre>
<strong>※ Development Period:</strong> 2023.09.12 ~ 2023.09.14 (9.5h) (Prototype)
                       2024.01.07 ~ 2024.01.08 (20h)
</pre>

<br>   


## Project Details (프로젝트 세부 주제)

Restoration of World War II Black and White Photographs_Attempts at Color Recovery through GAN Model Implementation. <br> <br>
![1  nyd8rtque7oa1](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/a1b68d32-d63e-4318-9f2a-c559f6755f23)

<br>

##  Utilized Model Architectures (사용된 모델 아키텍처)

- **Simple CNN :** A basic model for image classification tasks that used simple convolutional and pooling layers.

- **Deep CNN :** Implemented deeper convolutional layers to extract more complex image features.

- **Autoencoder :** Learned low-dimensional representations of images and reconstructed the images based on this learning.

- **U-Net :** Used in image segmentation tasks, it efficiently conveyed features through symmetric expansion and contraction paths.

- **GAN :** Constructed a structure where a generator and a discriminator learn through competition, leading to the generation of new images. <br> <br>

​![2  조합도](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/1ace4bf5-b944-4c78-935a-da7fa10ba421)

<p align="center"><em><strong>Deep Learning Model's 'Network Structure Diagram' Used in This Project</strong></em></p>

<br> <br> <br>


## Technical Stack Details (기술 스택 세부사항)


- **TensorFlow & Keras :** The primary deep learning libraries used to build and train models.

- **Python :** Utilized for data preprocessing, modeling, learning pipelines, and analyzing results.

- **Matplotlib & OpenCV :** Libraries used for loading, transforming, and visualizing image data. Matplotlib was used to visualize results during the learning process, while OpenCV was applied in image preprocessing tasks.

- **Google Colab :** Accelerated model training and experimentation in a cloud-based development environment using T4-GPU acceleration.

​<br> <br>  
## Project expected direction (프로젝트 예상 진행방향)
<br>  

![3  흑백 사진 데이터 모음](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/0b2381e7-8f1f-4f38-af3c-f3b888724664)
<br>  
- **Dataset Scale and Necessity**  
A substantial amount of image data is required for a black and white/color image restoration project. Estimates suggest that a minimum of over 100,000 images may be needed for effective training and model performance evaluation. High-performance computing resources are essential for processing such large datasets, which pose limitations when working on standard personal computers.
<br> <br>

- **Resource and Tool Necessity**  
Consequently, there is a need for tools capable of efficiently training on extensive datasets that include complex real-life photos and simple geometric images. Utilizing cloud-based platforms or high-performance computing resources is necessary, and in such environments, more complex network architectures can be experimented with and optimized.
<br> <br>

- **Project Goal Setting**  
The project's goal is to improve the color restoration capability for complex real-life images. **Focusing on capturing contours and color restoration**, the project aims to **explore new approaches by designing and applying the GAN architecture.** Insights gained in this process are expected to significantly aid in future model performance improvements.
<br>


​

## Project Progress (프로젝트 진행 과정)

**Initial Prototype Results** <br>  
![4  도형 데이터 수집](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/44e47461-3660-4b87-9dab-709d75ed3d0d)

In the initial stages of the project, a prototype model was created using a **Convolutional Neural Network(CNN)** and **U-Net architecture**, trained on a **simple geometric dataset**. These basic models successfully **recognized image contours and partially restored color**.
<br> <br> <br>
​
![5  구모델 구현](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/2a45248c-3581-4daf-8284-7c7754e9ac8b)
<p align="center"><em><strong>(Left: CNN model / Right: U-Net model)</strong></em></p>

Consequently, while the CNN model showed sharp color restoration results for basic geometric images, the **U-Net demonstrated a more refined ability to restore color in complex images**, particularly **excelling in reproducing image textures and boundaries**.
<br> <br> <br> <br>
​
**Expansion to Advanced Modeling**

Building on the initial success of the prototype, the project expanded its objectives towards designing and training more sophisticated models. Complex networks such as **Deep CNN, Autoencoder**, and **GAN** were developed to better grasp intricate image features and attempt more accurate color restoration. The design and application of GAN were central experiments of the project, with images generated by GAN expected to play a significant role in gauging the project's potential success.
<br> <br> <br> <br>
​
**Design and Performance Review**

Prior to incorporating GAN, the project initially trained and evaluated the performance of the other four models.

​![6 4개 모델 그래프](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/dd15b663-15d4-426d-8834-81cc11f9b6a4)

This graph shows the results obtained from the first model training phase of the project. The prototype's initial success led to the **segmentation of the CNN model** into two variations, with the **Autoencoder** model also added following the **U-Net**. Validation loss measures how well a model predicts on data it has not seen, typically indicating better generalization performance when lower on the graph.
 <br> <br>
 
Comparing the validation loss results across models allowed for an assessment of their learning and generalization capabilities. While the U-Net model showed promise in the prototype for tasks like image segmentation, a review of the validation loss trends revealed that U-Net consistently maintained higher validation losses compared to other models. This indicates that the U-Net model might not be optimized for the current dataset and hyperparameter settings, highlighting the need for further training with a broader and more diverse dataset to improve results.
<br> <br> <br>
​
![7  4개 모델 재학습](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/1eb020d3-a594-437f-96ae-4b93dc97f092)

After shifting the training dataset from complex everyday photos to simpler geometric shapes, the models were retrained and re-evaluated. At this stage, **all four models showed substantial numerical improvements in training and validation losses**. Notably, the Deep CNN and U-Net models exhibited significant loss reductions and more stable validation accuracy results. This confirmed that **models optimize faster and perform better generalization when trained on less complex datasets**.
<br>  <br>


​

## GAN Design and Experimentation (GAN 설계 및 실험)
<br>
![9  생성자, 판별자](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/b066faab-8e1b-4426-a01f-4b5e5e9318ae)

- **GAN Configuration:** The GAN architecture was composed of two main networks: the **generator** and the **discriminator**. The generator was tasked with creating images from random noise, while the discriminator worked to distinguish between real and generated images.

​![10  gan](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/5941856e-e645-4c37-bd95-37a708db0ed6)

- **Learning Process:** The model was trained over three sets of epochs, monitoring the losses of both the generator and the discriminator to gauge the model's learning progression. Loss functions were carefully selected to fulfill GAN's learning objectives.

​![11  gan photo](https://github.com/pixelwizard2/Project.AI--ColorQuest---AI-s-Journey-in-Reviving-WWII-Imagery/assets/138272416/6dfaa6f4-c17d-4fd5-896f-4b90a8ba481e)

- **Result Analysis:** After training, the quality of images produced by the model was evaluated qualitatively. However, this evaluation revealed that **the model generated results falling short of expectations**. Early GAN training started with a balance of competition between the generator and discriminator, but over time, as the discriminator's performance improved, the generator's loss increased. As the training progressed into the long term, this disparity grew, leading to a stagnation in the generator's development and ultimately resulting in significantly lower quality of the generated images. This underscores the **importance of maintaining a balance in GAN's learning process** and suggests a **need for strategies to harmonize these two networks** in future learning directions.

​

​

Conclusion and Reflections

​

While the project demonstrated the capability to design and experiment with GAN, the final outcomes were not satisfactory in creating color images from complex real-life black and white photographs. Particularly, the quality assessment of generated images showed that the GAN model still requires improvement.

​

Moreover, the prototypes implemented early in the project successfully converted basic black and white images into color, but the four more complex models designed in this project did not show a significant improvement over the initial success. This indicates that the anticipated performance enhancements were not achieved with increased complexity, emphasizing the need to strike a proper balance between model complexity and efficiency. The fact that the models could not handle datasets as extensive as desired to produce impactful results remains a significant disappointment of the project.

​

​

Future Learning Directions

​

Future research will need to improve the quality and quantity of datasets. Additionally, adjusting the model architecture and learning parameters to achieve more refined color restoration outcomes will be explored. A deeper understanding of GAN, along with improving the quality of training data, will be crucial. We are committed to successfully converting black and white photos into color with minimal datasets and model performance.

​

​

References

Python Official Documentation

Google Image Search Dataset

Official Documentation for TensorFlow and Keras
