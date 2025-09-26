# 🐱🐶 Cat vs Dog Classifier
#
# 📌 Proje Hakkında
# Bu proje, derin öğrenme tabanlı görüntü sınıflandırma problemi üzerine geliştirilmiştir.
# Amaç, verilen bir görselin kedi 🐱 mi yoksa köpek 🐶 mi olduğunu tahmin eden bir yapay zeka modeli tasarlamaktır.
#
# Kullanılan yöntemler:
# - ✅ Convolutional Neural Network (CNN)
# - ✅ Transfer Learning (EfficientNetB0)
# - ✅ Data Augmentation (çevirme, döndürme, zoom vb.)
# - ✅ Early Stopping & Model Checkpoint
#
# ⚙️ Kullanılan Teknolojiler
# - Python 🐍
# - TensorFlow / Keras
# - OpenCV
# - Matplotlib & Seaborn
# - NumPy & Pandas
#
# 📂 Dataset
# Proje, Kaggle’dan alınan Cat & Dog Dataset ile gerçekleştirilmiştir.
# 📌 Dataset linki: https://www.kaggle.com/datasets
# Dataset Train/Validation/Test olarak ayrılmıştır.
#
# 🏗️ Model Mimarisi
#
# 1. CNN (Scratch Model)
# - Conv2D + MaxPooling2D blokları
# - Flatten + Dense katmanlar
# - Dropout ile overfitting azaltma
#
# 2. Transfer Learning (EfficientNetB0)
# - EfficientNetB0 tabanı (ImageNet ağırlıkları ile)
# - GlobalAveragePooling2D
# - Dense (128, ReLU) + Dropout(0.3)
# - Dense (1, Sigmoid) → Binary Classifier
#
# 📊 Eğitim Süreci
# - Optimizer → Adam
# - Loss → Binary Crossentropy
# - Metric → Accuracy, Precision, Recall
# - Epoch → 20 (EarlyStopping ile durduruldu)
#
# 📈 Eğitim grafikleri:
# (örnek: training_plot.png buraya eklenebilir)
#
# 🧾 Sonuçlar
# - Accuracy ≈ %55–60 (küçük dataset nedeniyle sınırlı başarı)
# - Model bazı örneklerde doğru, bazılarında yanlış sınıflandırma yapmıştır.
# - Daha büyük dataset ve fine-tuning ile başarı %90+ seviyelerine çıkabilir.
#
# 🖼️ Test Örneği
# Tahmin Skoru: 0.87
# 👉 Tahmin Sınıfı: Köpek 🐶
#
# 🔮 Gelecek Çalışmalar
# - Daha büyük dataset ile eğitim
# - VGG16, ResNet gibi farklı transfer learning modelleri
# - Veri artırma (augmentation) yöntemlerini genişletme
# - Modeli web arayüzü veya mobil uygulamaya deploy etme
