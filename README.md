# regnet_re  
----------------------------------  
## 0322:  
- 读了regnet的论文；  
- 修改了regnet中的一些参数；  
- 整理了数据集  
## 0323：  
- 训练结束，获得.pth权重文件，训练的日志放在0322.log中  
- 使用eval.py评估了一下模型，发现误差很大，评估的日志放在0323_eval.log中  
- 可视化一下结果:使用inference.py  
![image](https://github.com/XxxuLimei/regnet_re/blob/main/pic/Figure_1.png)  
![image](https://github.com/XxxuLimei/regnet_re/blob/main/pic/Figure_1_inference.png)  
![image](https://github.com/XxxuLimei/regnet_re/blob/main/pic/Figure_2_inference.png)  
- 评估的结果如下：  
```
(base) xilm@xilm-MS-7D17:~/fuxian/regnet-master$ python inference.py 
Dataset size: 15310
Trained until Epoch: 49
GT Decalib Angles: [-4.80459283 -0.5668939  -2.75898791]
GT Decalib Translations: [-0.20128943 -0.30675429  0.25836912]
Pred Decalib Angles: [-4.92227933  0.4895953  -2.30273136]
Pred Decalib Translations: [-0.20907906 -0.2878651   0.23827842]
Roll Error 1.0616891896029208
Pitch Error 0.45584506865678576
Yaw Error 0.060402471164707865
X Error 0.0256218173250991
Y Error 0.03270152958117632
Z Error 0.010479456132357956
Mean Rotational Error 0.5259789098081381
Mean Translational Error 0.022934267679544457
Init Roll Error 0.3010312660418041
Init Pitch Error 2.723561356765938
Init Yaw Error 4.854953615026127
Init X Error 0.3242752623554779
Init Y Error 0.2646799656724974
Init Z Error 0.19984741859357008
Mean Rotational Error 2.62651541261129
Mean Translational Error 0.26293421554051516
GT Decalib Angles: [-2.30947414 -0.12397342 -4.04833463]
GT Decalib Translations: [-0.04584581 -0.16278234 -0.12571678]
Pred Decalib Angles: [-1.91241827  0.5741674  -4.29402617]
Pred Decalib Translations: [-0.074084   -0.09309605 -0.14601445]
Roll Error 0.664863438984017
Pitch Error 0.2517155833337749
Yaw Error 0.44954897127647236
X Error 0.06852665088307908
Y Error 0.022677438647334736
Z Error 0.023977342324179696
Mean Rotational Error 0.45537599786475474
Mean Translational Error 0.038393810618197834
Init Roll Error 0.055886006264826704
Init Pitch Error 4.0149894569572
Init Yaw Error 2.375796925395663
Init X Error 0.18467869995381447
Init Y Error 0.12414813531195185
Init Z Error 0.04995209952547963
Mean Rotational Error 2.148890796205897
Mean Translational Error 0.11959297826374865
GT Decalib Angles: [-4.6517029   4.45596535  2.11318117]
GT Decalib Translations: [-0.3932409  -0.27346969 -0.48459673]
Pred Decalib Angles: [-4.7066172   5.27578678  0.71560206]
Pred Decalib Translations: [-0.47848171 -0.19227648 -0.53488749]
Roll Error 0.8169979039204038
Pitch Error 1.39282105356551
Yaw Error 0.07947163638759473
X Error 0.06618700287398592
Y Error 0.05559760232726976
Z Error 0.06676740077689991
Mean Rotational Error 0.763096864624503
Mean Translational Error 0.0628506686593852
Init Roll Error 4.306196851687311
Init Pitch Error 2.5327049236997885
Init Yaw Error 4.571275857227178
Init X Error 0.2667873128301038
Init Y Error 0.4990183567856524
Init Z Error 0.40899674303574596
Mean Rotational Error 3.8033925442047596
Mean Translational Error 0.3916008042171674
GT Decalib Angles: [ 2.94016627 -1.99756955  0.77865662]
GT Decalib Translations: [-0.20305014  0.29968798  0.12660311]
Pred Decalib Angles: [ 3.05955385 -1.37137759  0.87561125]
Pred Decalib Translations: [-0.22437114  0.2910105   0.10556356]
Roll Error 0.6269626374225374
Pitch Error 0.09899785712944216
Yaw Error 0.1159403977421279
X Error 0.010713756480996837
Y Error 0.028758923312134643
Z Error 0.017541017660097358
Mean Rotational Error 0.28063363076470255
Mean Translational Error 0.019004565817742947
Init Roll Error 1.9777972531146237
Init Pitch Error 0.8382346725373939
Init Yaw Error 2.936275722401593
Init X Error 0.30872636528360314
Init Y Error 0.1388867717359074
Init Z Error 0.19639052006597374
Mean Rotational Error 1.917435882684537
Mean Translational Error 0.21466788569516146
GT Decalib Angles: [-3.32604534 -4.80840679 -4.14441731]
GT Decalib Translations: [0.32299128 0.37611288 0.33439368]
Pred Decalib Angles: [-2.84150965 -4.18054093 -3.16895353]
Pred Decalib Translations: [0.29400983 0.3882395  0.31270492]
Roll Error 0.5877598210602069
Pitch Error 1.0079117229454138
Yaw Error 0.5363807649737196
X Error 0.01076086936172118
Y Error 0.0291408914070954
Z Error 0.026675756363926162
Mean Rotational Error 0.7106841029931134
Mean Translational Error 0.022192505710914245
Init Roll Error 4.534065585825827
Init Pitch Error 4.363734365953959
Init Yaw Error 3.425478165869065
Init X Error 0.34959622154511594
Init Y Error 0.3526247745060588
Init Z Error 0.33479793692464455
Mean Rotational Error 4.107759372549617
Mean Translational Error 0.34567297765860644
```  

## Reference:  
RegNet:[Link](https://github.com/aaronlws95/regnet)  
