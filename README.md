# 🚗 Araç Fiyat Tahmini Projesi

Bu proje, makine öğrenmesi algoritmaları kullanılarak araçların fiyatlarını tahmin etmek amacıyla geliştirilmiştir. Veri bilimi pipeline'ının (EDA, Preprocessing, Modelling) temel adımlarını içerir.

## 🎯 Proje Amacı
Veri setindeki `Yıl`, `Kilometre`, `Vites Tipi` ve `Yakıt Tipi` gibi özellikleri kullanarak aracın piyasa değerini tahmin eden bir **Lineer Regresyon** modeli oluşturmak.

## 🛠️ Kullanılan Teknolojiler
* **Python:** Veri analizi ve modelleme dili.
* **Pandas & NumPy:** Veri manipülasyonu.
* **Matplotlib & Seaborn:** Veri görselleştirme (Korelasyon matrisi, Scatter plot).
* **Scikit-Learn:** Makine öğrenmesi modeli (Linear Regression) ve eğitim/test ayrımı.

## 📊 Analiz Sonuçları
* **Veri Temizliği:** Aykırı değerler (Outliers) IQR ve Quantile yöntemleriyle temizlendi.
* **Özellik Dönüşümü:** Kategorik veriler (Vites, Yakıt) sayısal verilere (Encoding) dönüştürüldü.
* **Model Başarısı:** Model, mevcut verilerle **%45** civarında bir R² skoru elde etmiştir.
    * *Not:* Başarının bu seviyede kalmasının temel nedeni, veri setinde 'Marka/Model' bilgisinin modele dahil edilmemiş olmasıdır. İlerde oluşturulacak versiyonlarda bu özellik eklendiğinde başarının artması beklenmektedir.

## 🚀 Gelecek Hedefleri (v2.0)
* Marka ve Model sütunlarının analize dahil edilmesi.
* Random Forest veya XGBoost gibi daha gelişmiş modellerin denenmesi.

## 📊 Analiz Sonuçları (Güncelleme v1.1)
* **Marka Puanlama:** Markalar lüks/ekonomik algısına göre 4 farklı segmente ayrıldı ve puanlandı (Feature Engineering).
* **Başarı Artışı:** Bu yeni özelliğin eklenmesiyle modelin R² skoru **%45'ten %59.12'ye** yükselmiştir.
* **Gözlem:** Marka bilgisinin fiyat üzerindeki etkisi, Kilometre bilgisinden çok daha belirleyici çıkmıştır.

---
*Bu proje Ergün Üngör tarafından geliştirilmiştir.*
