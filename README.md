# Leaf Disease Prediction
# Inspiration:
I have been always thinking to explore the field og agriculture and build an automatic disease prediction model and deploy it. After continuous web surfing I came across a reasearch article by rishnaswamy Rangarajan Aravind & Purushothaman Raja which opened doors for my project. 
Article link: https://doi.org/10.1080/00051144.2020.1728911

# Stage 1

Downloaded the rice leaf dataset from kaggle and worked on it to predict four types of rice leaf. The dataset had high definition images and I had to compress the images into lower dimensions to avoid huge computational cost.
Built various models of image sizes 128,150,175 and 200 using a custom neural network and transfer learning techniques, Inception V3, ResNet, VGG16,VGG19. All of them resulted in test accuracy less than 60%.

Dataset link: https://www.kaggle.com/shayanriyaz/riceleafs

# Stage 2
Found a dataset on kaggle called Plant Village which consists of 15 types of plant disease types. 
Build models to predict these plat disease types. I have tried with varioud image sizes and epochs by setting learning rate are 0.0003. I have also used tranfer learning techniques such as Inception V3 and ResNet. Below are the reports of my trials.

Dataset link: https://www.kaggle.com/emmarex/plantdisease

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
  
  
