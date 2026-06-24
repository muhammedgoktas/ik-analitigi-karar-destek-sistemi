# 🎯 İK Analitiği Karar Destek Sistemi ve Çalışan Devir Hızı Tahmini

Bu proje, şirketlerin İnsan Kaynakları verilerini kullanarak çalışanların işten ayrılma (attrition) olasılıklarını tahmin eden, çalışan profillerini analiz eden ve İK yöneticilerine proaktif kararlar almalarında yardımcı olan uçtan uca bir makine öğrenimi çözümüdür.

## 🚀 Öne Çıkan Özellikler

- **Veri Sızıntısını Önleyen Boru Hattı (Pipeline):** Eksik veri doldurma, ölçeklendirme (MinMaxScaler) ve dengesiz veri setini aşırı örnekleme (SMOTE) işlemleri, veri sızıntısını önlemek amacıyla profesyonel bir standart olan `imblearn.pipeline` içinde yapılandırılmıştır.
- **Ayrılma Riski Tahmini (Risk Scoring):** Lojistik Regresyon modeli ile her bir çalışanın işten ayrılma olasılığı (%) hesaplanmış ve en riskli çalışanlar hedeflenebilir bir eylem planı için raporlanmıştır.
- **Açıklanabilir Yapay Zeka (Explainable AI) ile Kümeleme:** K-Means algoritması ile çalışanlar stratejik gruplara ayrılmış; ardından bu kümelerin karakteristik özellikleri Karar Ağaçları (Decision Tree) ile if-else kurallarına dökülerek İK uzmanları için somut ve "anlaşılır" bir formata dönüştürülmüştür.
- **Otomatik PDF Raporlama:** Elde edilen veriler, model sonuçları ve içgörüler, `ReportLab` kütüphanesi kullanılarak yöneticilere sunulmaya hazır, düzenli bir PDF dosyasına otomatik olarak basılmaktadır.

## 📊 Veri Seti
Projede kullanılan veri seti çalışanlara ait şu öznitelikleri (features) içermektedir:
- Memnuniyet seviyesi ve Son performans değerlendirme notu
- Çalıştığı proje sayısı ve Ortalama aylık çalışma saati
- Şirkette geçirdiği süre
- İş kazası geçmişi, departmanı ve maaş seviyesi

## 🛠️ Kullanılan Teknolojiler
- **Veri İşleme:** `pandas`, `numpy`
- **Makine Öğrenimi:** `scikit-learn`, `imbalanced-learn`
- **Veri Görselleştirme:** `matplotlib`, `seaborn`
- **Raporlama:** `reportlab`

EKRAN GÖRÜNTÜLERİ :

<img width="1075" height="514" alt="image" src="https://github.com/user-attachments/assets/8667fa4f-4986-429d-9402-be8edc9147d2" />

<img width="1069" height="744" alt="image" src="https://github.com/user-attachments/assets/d6ff4718-59a0-4361-9c36-3a00b8ba1b89" />

<img width="1079" height="677" alt="image" src="https://github.com/user-attachments/assets/af42834d-7737-460b-9977-906c4bcf0868" />

<img width="1090" height="573" alt="image" src="https://github.com/user-attachments/assets/3d3d4b1a-5e8b-42da-b0bb-b9ee763d3b3d" />

<img width="1104" height="486" alt="image" src="https://github.com/user-attachments/assets/92b71dac-9120-443b-97a0-b7cd755ee1ae" />

<img width="1099" height="495" alt="image" src="https://github.com/user-attachments/assets/00799584-6625-43d9-a8d1-1768e84a0fce" />

<img width="1117" height="665" alt="image" src="https://github.com/user-attachments/assets/2b845f7b-bae9-4f1c-bde3-a0b67bf1656e" />

<img width="1123" height="713" alt="image" src="https://github.com/user-attachments/assets/eeb49f48-db49-4bfa-a2cf-203d52f0f557" />

<img width="1101" height="645" alt="image" src="https://github.com/user-attachments/assets/bb5a1fc4-f40a-4b6f-bb23-1d95233d0fea" />

<img width="1110" height="667" alt="image" src="https://github.com/user-attachments/assets/4b5838c3-754d-4b83-a450-82226a0f8214" />

<img width="1104" height="654" alt="image" src="https://github.com/user-attachments/assets/bb50890c-beaa-4f1f-b139-5d64ad23f421" />

<img width="1075" height="328" alt="image" src="https://github.com/user-attachments/assets/801b5721-953f-4fb1-8f2c-d93964ff722f" />

<img width="1116" height="135" alt="image" src="https://github.com/user-attachments/assets/1f36cbf3-8be6-4011-8583-23502349f669" />

<img width="1094" height="281" alt="image" src="https://github.com/user-attachments/assets/17eefe2d-3619-43cd-ad57-5186bfd9185d" />

<img width="1106" height="260" alt="image" src="https://github.com/user-attachments/assets/5c302425-1b10-4e20-860f-fcec59876f4d" />

Rapor pdf görselleri :
<img width="1914" height="888" alt="image" src="https://github.com/user-attachments/assets/49787d96-e7c5-4fbf-8830-a9b47668c399" />

<img width="1894" height="819" alt="image" src="https://github.com/user-attachments/assets/b06c4fed-772b-4c05-b994-154b881edfbd" />


## ⚙️ Kurulum ve Çalıştırma

Projeyi kendi ortamınızda test etmek için aşağıdaki adımları izleyebilirsiniz:

1. **Repoyu klonlayın:**
   ```bash
   git clone https://github.com/muhammedgoktas/ik-analitigi-karar-destek-sistemi.git
   cd ik-analitigi-karar-destek-sistemi
   ```

2. **Gerekli kütüphaneleri yükleyin:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Projeyi çalıştırın:**
   Jupyter Notebook ortamında `İK_ANALİTİĞİ_PROJESİ.ipynb` dosyasını açarak analizleri inceleyebilir ve model sonuçlarını yeniden üretebilirsiniz.

## 📬 İletişim
**Muhammed Mustafa Göktaş**
- [LinkedIn](https://www.linkedin.com/in/mmgbilisim)
- [GitHub](https://github.com/muhammedgoktas)
