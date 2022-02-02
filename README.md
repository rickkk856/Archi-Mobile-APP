# Archi-Mobile-APP

[Download the .apk here](https://drive.google.com/file/d/1f2yyUsiMGyjA2XdsyaHhP1diAn3c9Omg/view?usp=sharing)

<!-- ABOUT THE PROJECT -->
## About The Project 

This mobile app is based on the image recognition task of architectural styles, the training phase used more than 4000 images from the paper ["Architectural Style Classification using Multinomial Latent Logistic Regression"](https://www.kaggle.com/dumitrux/architectural-styles-dataset?select=README.txt) (ECCV2014), made by Zhe Xu. However not all the styles were considered. 

The model was trained on [lobe ai](https://lobe.ai/) and used more than 6 thousand images, with 80% of train data + 20% of test data, we achieved 98% of accuracy on ResNet-50V2 (optimized for acc%), and 84% of accuracy on MobileNetV2 (optimized for speed). The Android APP uses tensorflow lite, hence, it is recomended to optmize for speed.

| Architectural Style | Number of Samples | MobileNetV2 (100%) | MobileNetV2 (20%) | ResNet-50V2(100%) | ResNet-50V2(20%) |
| --- | --- | --- | --- | --- | --- |
| Art Deco architecture | 724 | 670% | 67% | 98% | 94% |
| Art Nouveau architecture | 855 | 94% | 89% | 98% | 93% |
| Gothic architecture | 210 | 100% | 100% | 100% | 100% |
| Baroque architecture | 471 | 85% | 83% | 98% | 98% |
| Byzantine architecture | 213 | 89% | 88% | 100% | 100% |
| Romanesque architecture | 208 | 91% | 90% | 95% | 88% |
| Palladian architecture | 220 | 84% | 70% | 95% | 86% |
| Greek Revival architecture | 622 | 96% | 93% | 99% | 97% |
| Novelty architecture | 418 | 95% | 93% | 99% | 99% |
| Bauhaus architecture | 169 | 79% | 70% | 98% | 88% |
| Chicago school architecture | 292 | 89% | 79% | 99% | 97% |
| Beaux-Arts architecture | 376 | 47% | 29% | 98% | 93% |
| Postmodern architecture | 418 | 90% | 89% | 99% | 98% |
| Deconstructivism | 418 | 90% | 89% | 99% | 98% |
| International style | 408 | 46% | 42% | 100% | 96% |
| Parana's Northern Colonial Architecture | 394 | 97% | 91% | 99% | 96% |
| **Total Number of Imgs and Average Acc%** | **6348** | **84%** | **79%** | **98%** | **95%** |


## How to Use?
Download the App from this [link](https://drive.google.com/file/d/1f2yyUsiMGyjA2XdsyaHhP1diAn3c9Omg/view?usp=sharing) and install `Archi-Mobile-APP.apk` on your phone. You may have to change configuration settings to allow instalation, or try it on a virtual machine.  

![Sem nome](https://user-images.githubusercontent.com/62864640/116631319-343c7f80-a92b-11eb-9f41-baa27735d362.png)

If you want to try the model on other platforms you may use the files on `tflite` folder. 

_PS: The [android-bootstrap template](https://github.com/lobe/android-bootstrap) offered by microsoft still needed to have few changes like setting `camera!!.setDisplayOrientation(90)` to `(0)` [here](https://github.com/lobe/android-bootstrap/blob/d94b4803ade037b509d561239ae0054c126d4401/lobe_android/app/src/main/AndroidManifest.xml#L21) and setting             `android:configChanges="orientation"` + `android:screenOrientation= "fullSensor"` after this [line](https://github.com/lobe/android-bootstrap/blob/d94b4803ade037b509d561239ae0054c126d4401/lobe_android/app/src/main/java/com/example/test/LegacyCameraConnectionFragment.kt#L201)_

_Lobe is a free beta machine learning software currently under development by Microsoft_

_This app was made on Lobe AI and Android-bootstrap and Android Studio_


## Citation
```
@article{Rodrigues2021,
abstract = {In the last decades, studies on cultural heritage have been interpreted as a complex and multifaceted phenomenon, in which heritage is no longer understood as just an isolated sector, but as an integral part of the city. In this context, the physical-digital environments of Smart Cities are inserted, which aim to increase this connectivity through data and interfaces, proposing innovative solutions. In this sense, we propose an artifact as an interaction interface between man-machine-medium, which identifies the typical wooden houses of the colonization in the North of Paran{\'{a}}, within a diversity of architectural styles, in order to enhance the user's perception in terms of continuity between the city and heritage. For this, a pilot study was developed in which an Artificial Intelligence model was trained for the recognition of building patterns with computer vision. Finally, the results show that the model obtained an accuracy compatible with those presented in the state of the art, and has the potential to generate user engagement with heritage, technological transfer and future mapping of historic buildings, data that is potentially useful for the delineation of intervention plans at the macro-urban scale.},
address = {Londrina},
author = {Rodrigues, Ricardo Cesar; Wedekin, Gabriela Oliveira; Henning, Priscila; Duarte, Rovenir Bertola},
journal = {VII Simp{\'{o}}sio Brasileiro de Qualidade do Projeto no Ambiente Constru{\'{i}}do},
keywords = {Computer vision,North of Paran{\'{a}}.,architectural style,artificial intelligence,built heritage},
pages = {11},
publisher = {Associa{\c{c}}{\~{a}}o Nacional de Tecnologia do Ambiente Constru{\'{i}}do (ANTAC)},
title = {{Architectural Style Classification Via Mobile Application and the Wooden Houses in the North of Paran{\'{a}}}},
year = {2021}
url = {https://www.researchgate.net/publication/356277224_Classificacao_de_Estilo_Arquitetonico_via_Aplicativo_Mobile_e_as_Casas_de_Madeira_no_Norte_do_Parana}
}
```

