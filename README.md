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