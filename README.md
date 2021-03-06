# Brain-Tumor-Detection-Classifier

## 背景介紹:
建構以深度學習分辨腦部斷層掃描片中是否長有腦瘤的模型，學習影像分為Brain Tumor(腦瘤)、Normal(正常)兩種。

![image](https://github.com/tddwso/Brain-Tumor-Detection-Classifier-by-Deep-Learning/blob/main/pic2.PNG)

## 預計完成目標:
以卷積神經網絡(Convolutional Neural Network)學習分辨Brain Tumor及Normal。
運用Transfer Learning(遷移式學習)，將他人訓練好的(pre-trained model)參數複製過來，當作我們模型參數，
使用的模型: VGG16，VGG 是英國牛津大學 Visual Geometry Group 的縮寫，主要貢獻是使用更多的隱藏層，大量的圖片訓練，提高準確率至90%。
## 資料集:
Train Data : 243
## 使用環境:
Python 3.8

TensorFlow 2.3.1 
## 訓練和測試結果
最佳模型訓練準確度84% 

![image](https://github.com/tddwso/Brain-Tumor-Detection-Classifier-by-Deep-Learning/blob/main/ACC.PNG)

ROC曲線 (Receiver operating characteristic curve) & AUC (Area Under Curve)

ROC曲線會以對角線為基準，曲線下的面積(AUC)來判別ROC曲線的鑑別力，AUC數值的範圍從0到1，數值愈大，代表模型的鑑別力越好。

![image](https://github.com/tddwso/Brain-Tumor-Detection-Classifier-by-Deep-Learning/blob/main/ROC.png)

實際測試結果

![image](https://github.com/tddwso/Brain-Tumor-Detection-Classifier-by-Deep-Learning/blob/main/test.PNG)

## 使用Streamlit App展示成果

![image](https://github.com/tddwso/Uniqlo-Label-Defect-Classification-by-Deep-Learning/blob/main/Stream%20Logo.png)

Streamlit 是一個開源Python函式庫，可以快速製作Data App。

實作影片(以下圖片為Youtube影片連結)

APP操作方法:

1.開啟資料夾選取想要測試的影像

2.APP執行影像辨識

3.顯示辨識結果
[![IMAGE ALT TEXT HERE](https://github.com/tddwso/Brain-Tumor-Detection-Classifier-by-Deep-Learning/blob/main/streamlit.PNG)](https://youtu.be/BFt50DN1uzE)


