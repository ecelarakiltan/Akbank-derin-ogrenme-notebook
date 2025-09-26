# Akbank-derin-ogrenme-notebook

# Derin Öğrenme Bootcamp Projesi – CNN ile Görüntü Sınıflandırma

📌 Giriş

Bu proje, Akbank Derin Öğrenme Bootcamp kapsamında geliştirilmiştir. Projede amaç, mimari unsurların (kemer, sütun, kubbe, vb.) yer aldığı görüntüleri sınıflandırmak için CNN (Convolutional Neural Network) mimarisini kullanmaktır.

Seçilen veri seti: Architectural Heritage Elements Image64

Sınıf sayısı: 10
Toplam görüntü: ~15.000
Projede yalnızca supervised öğrenme yaklaşımı kullanılmıştır.

🧰 Kullanılan Yöntemler ve Teknikler

Framework: PyTorch
Veri Önişleme:
Resize ve Normalize işlemleri
Data Augmentation (Rotation, Flip, Zoom, Color Jitter)
CNN Model Mimarisi:
Convolutional Layers + Pooling Layers
Dropout (Overfitting önlemek için)
Fully Connected (Dense) Layers
Aktivasyon fonksiyonları: ReLU, Softmax
Hiperparametreler:
Learning Rate: 0.001
Batch Size: 32
Dropout Oranı: 0.3
Epoch: 30
Model Eğitimi ve Değerlendirme:
Train ve Validation Loss/Accuracy grafikleri
Confusion Matrix ve Classification Report
WeightedRandomSampler ile sınıf dengesizliği çözümü
📈 Sonuçlar

Model Başarı Skoru (Accuracy): 0.7272
Confusion Matrix ve Sınıflar Arası Dağılım: Notebook içerisinde görselleştirilmiştir.
Overfitting riski düşük, model genel doğruluk ve F1-score bakımından tatmin edici sonuçlar vermektedir.
Önemli: Bazı sınıflar az sayıda örnek içerdiği için modelin tahmin performansı sınıf bazında farklılık gösterebilir. WeightedRandomSampler ile bu durum minimize edilmiştir.
🔧 Gelecek Çalışmalar

Model mimarisini derinleştirerek veya filtre sayılarını artırarak doğruluk iyileştirilebilir.
Transfer Learning (ResNet, EfficientNet vb.) uygulanabilir.
Streamlit veya Gradio ile basit bir UI üzerinden gerçek zamanlı sınıflandırma yapılabilir.
Daha büyük veri setleri ve gerçek zamanlı veri akışı ile model performansı artırılabilir.
🔗 Kaggle Notebook Linkleri
