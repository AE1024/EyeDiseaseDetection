Göz Hastalıkları Sınıflandırma Projesi (Eye Disease Classification)
Bu proje, fundus (göz dibi) fotoğraflarını analiz ederek farklı göz hastalıklarını (Glokom, Katarakt, Diyabetik Retinopati) ve normal göz yapılarını sınıflandırmak amacıyla geliştirilmiş bir derin öğrenme çalışmasıdır. Proje kapsamında geleneksel CNN mimarileri ile modern Transfer Learning (Transfer Öğrenme) teknikleri karşılaştırılmıştır.

## 📊 Veri Seti Hakkında
Veri seti, göz dibi görüntülerinden oluşmakta ve aşağıdaki kategorileri içermektedir:

Glaucoma (Glokom)

Cataract (Katarakt)

Diabetic Retinopathy (Diyabetik Retinopati)

Normal

Görüntüler ön işleme aşamasında yeniden boyutlandırılmış ve eğitim performansını artırmak için normalize edilmiştir.

## 🚀 Kullanılan Modeller ve Teknikler
Projede üç farklı yaklaşım test edilmiştir:

### CNN Mimarisi
Sıfırdan tasarlanmış, ardışık Conv2D, MaxPooling2D ve Dense katmanlarından oluşan temel bir model.

### EfficientNetB0 (Transfer Learning) 
Önceden ImageNet veri setiyle eğitilmiş EfficientNetB0 mimarisi kullanılarak özellik çıkarımı yapılmıştır.

### EfficientNetB0 (Fine-Tuning)
Transfer öğrenme modelinin son katmanları, bu spesifik veri setine uyum sağlaması için ince ayar (fine-tuning) işlemine tabi tutulmuştur.

🛠️ Kurulum
Projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1 - Depoyu klonlayın

    git clone https://github.com/AE1024/goz-hastaliklari-siniflandirma.git
2 - Gerekli kütüphaneleri yükleyin

    pip install -r requirements.txt
3 - Veri Seti 
    https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification

Eye Disease Classification Project
This project is a deep learning study developed to classify different eye diseases (Glaucoma, Cataract, Diabetic Retinopathy) and normal eye structures by analyzing fundus (back of the eye) images. The project compares traditional CNN architectures with modern Transfer Learning techniques.

## 📊 About the Dataset
The dataset consists of fundus images and includes the following categories:

Glaucoma

Cataract

Diabetic Retinopathy

Normal

The images were resized and normalized during the preprocessing phase to improve training performance.

## 🚀 Models and Techniques Used
Three different approaches were tested in the project:

### CNN Architecture
A basic model designed from scratch, consisting of successive Conv2D, MaxPooling2D, and Dense layers.

### EfficientNetB0 (Transfer Learning)

Feature extraction was performed using the EfficientNetB0 architecture, previously trained with the ImageNet dataset.

### EfficientNetB0 (Fine-Tuning)
The final layers of the transfer learning model were fine-tuned to adapt to this specific dataset.

🛠️ Setup
To run the project in your local environment, you can follow these steps:

1 - Clone the repository

git clone https://github.com/AE1024/goz-hastaliklari-siniflandirma.git
2 - Install the necessary libraries

pip install -r requirements.txt
3 - Dataset
https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification
