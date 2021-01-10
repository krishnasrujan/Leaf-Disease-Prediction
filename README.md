# Leaf Disease Prediction

# Motivation
I have been always thinking to explore the field of agriculture and build an automatic disease prediction model and deploy it. After continuous web surfing I came across a reasearch article by Krishnaswamy Rangarajan Aravind & Purushothaman Raja which opened doors for my project. 
Article link: https://doi.org/10.1080/00051144.2020.1728911

# Stage 1

Downloaded the rice leaf dataset from kaggle and worked on it to predict four types of rice leaves. The dataset had high definition images and I had to compress the images into lower dimensions to avoid huge computational cost.
Built various models using image sizes 128,150,175 and 200 using a custom neural network and transfer learning techniques such as Inception V3, ResNet, VGG16, VGG19. All of them resulted in test accuracy less than 60%.

Dataset link: https://www.kaggle.com/shayanriyaz/riceleafs

# Stage 2
Found a dataset on kaggle called Plant Village which consists of 15 types of plant diseases. 
Dataset link: https://www.kaggle.com/emmarex/plantdisease

Buildt model to predict these plat disease types. I have tried with various image sizes and epochs by setting learning rate as 0.0003. I have also used tranfer learning techniques such as Inception V3 and ResNet. Below are the reports of my trials.


  # Custom Built Model
  Model Summary
  
  <img width="263" alt="custom_model summary " src="https://user-images.githubusercontent.com/48923446/94246401-51dedc00-ff39-11ea-9f9d-4098fe9c2bd0.png">
  
  Model Report
  
  <img width="382" alt="15_custom_report " src="https://user-images.githubusercontent.com/48923446/94246468-66bb6f80-ff39-11ea-9223-b7d46eec378a.png">
  
  # ResNet50
  Model Summary 
  
  <img width="354" alt="inception_15 model" src="https://user-images.githubusercontent.com/48923446/94248004-818ee380-ff3b-11ea-9267-70ed98c5832f.png">

  Model Report
  
  <img width="356" alt="resnet50_15_report" src="https://user-images.githubusercontent.com/48923446/94248328-f2360000-ff3b-11ea-8e30-aa52fd803368.png">

  # Inception V3
  
  Model Report 
  
  <img width="359" alt="inception v3_15_report " src="https://user-images.githubusercontent.com/48923446/94248195-c0bd3480-ff3b-11ea-99ed-afb3419467a0.png">
  
 
 # Stage 3 
 Found a new plant village dataset on kaggle which consists of 38 classes of plant disease types. 
 I merged the rice leaf dataset(only healthy and unhealthy classes) with this dataset which resulted in 40 classes totally. 
 Kept the image size as 128 pixels and created train dataset of 400 images in each class and validation dataset of 200 images in each class(the rice leaf classes in 
 validation dataset have only 100 images each).
 
 Trained it in custome built model, VGG16, VGG19, Inception V3. Achived best results using VGG16 model with 98% training accuracy and 92.3% validatioon accuracy.
 
 Note : Leaky relu and relu are performing very poor on this dataset so used sigmoid actuvation function for hidden layers.
 
 # Custom Model 
  Model Summary
  
  <img width="314" alt="custom_40" src="https://user-images.githubusercontent.com/48923446/94252190-35df3880-ff41-11ea-8b00-a6dcd0539209.png">
  
  Model Report
  
  <img width="826" alt="custom_40_report" src="https://user-images.githubusercontent.com/48923446/94255682-3fb76a80-ff46-11ea-9827-c702e8aa9798.png">
  
# Inception V3
Model Summary

<img width="272" alt="inceptrioon40_summary" src="https://user-images.githubusercontent.com/48923446/94253152-82774380-ff42-11ea-86ec-5f68b4b78e7c.png">

Model Report 

<img width="720" alt="Incaption_40_report" src="https://user-images.githubusercontent.com/48923446/94256080-da17ae00-ff46-11ea-93b8-86955687c3a8.png">

# VGG19 
Model Summary

<img width="274" alt="vgg19_40_summary" src="https://user-images.githubusercontent.com/48923446/94253215-991d9a80-ff42-11ea-9364-4f3eeff826b9.png">

Model Report
VGG19 model's metrics were almost same with VGG16 model's metrics. But VGG16 model's validation accuracy was more and validation loss was less compared to VGG19 model.

# VGG16 
Model Summary 

<img width="266" alt="vgg16_40_summary" src="https://user-images.githubusercontent.com/48923446/94253313-c1a59480-ff42-11ea-8445-3693732ac4ab.png">

Model Report 

<img width="730" alt="latest plant metrics" src="https://user-images.githubusercontent.com/48923446/99278578-3c10d780-2855-11eb-8b64-21ffb7f5ebbe.PNG">

Loss and accuracy plots

<img width="303" alt="accuracy" src="https://user-images.githubusercontent.com/48923446/99528733-bb70e900-29c4-11eb-85d4-74d17ed54fc2.PNG">    <img width="292" alt="loss" src="https://user-images.githubusercontent.com/48923446/99528738-bd3aac80-29c4-11eb-93bb-709a2641a8cd.PNG">

# Useful Links:

I have dockerized the project. Link to docker repository: https://hub.docker.com/repository/docker/krishnasrujan/leaf_health_detection

LinkedIn: https://www.linkedin.com/in/krishna-srujan-139147168/
