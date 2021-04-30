# Archi-Mobile-APP

<!-- ABOUT THE PROJECT -->
## About The Project

The training phase used more than 4000 images from the paper ["Architectural Style Classification using Multinomial Latent Logistic Regression"](https://www.kaggle.com/dumitrux/architectural-styles-dataset?select=README.txt) (ECCV2014), made by Zhe Xu. However not all the styles were considered. 

The model was trained on [lobe](https://lobe.ai/) took appoximately 5 hours to train and + 4 hours to optmize model. 

With an 80% train data + 20% test data, we achieved 89% of accuracy optimizing for acc%, and 81% of accuracy setting to train for speed.The Android APP uses tensorflow lite, hence, it's optmized for speed and not work properly as on lobe since images are aren't resized inside the app.

Architectural Styles Supported
1. Art Deco architecture
1. Art Nouveau architecture
1. Baroque architecture
1. Bauhaus architecture
1. Beaux-Arts architecture
1. Byzantine architecture
1. Chicago school architecture
1. Deconstructivism
1. Gothic architecture
1. Greek Revival architecture
1. International style
1. Novelty architecture
1. Palladian architecture
1. Postmodern architecture
1. Queen Anne architecture
1. Romanesque architecture

## How to Use?
Download the repository and install `Archi-Mobile-APP.apk` on your phone. You may have to change configuration settings to allow instalation, or try it on a virtual machine.  
If you want to try the model on other platforms you may use the files on `tflite` folder

![Sem nome](https://user-images.githubusercontent.com/62864640/116631319-343c7f80-a92b-11eb-9f41-baa27735d362.png)

_Lobe is a free beta machine learning software currently in development by Microsoft_

_This app was made on Lobe and Android-bootstrap and Android Studio_

## Todo

Collect images of 'colonial wooden houses' from Londrina's city in Brazil, or other similar to this characteristic architectural heritage.

Re-train model with local image sub-set.

Distribute & have fun.
