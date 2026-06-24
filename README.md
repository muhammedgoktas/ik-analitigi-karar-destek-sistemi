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
