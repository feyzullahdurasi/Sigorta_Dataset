# Sigorta Ücreti Tahmini 📊

Bu proje, bir veri bilimi dersi vize ödevi kapsamında gerçekleştirilmiştir. Projenin amacı, bireylerin yaş, cinsiyet, vücut kitle indeksi (BMI), çocuk sayısı, sigara kullanımı ve yaşadığı bölge gibi demografik özelliklerine göre yıllık sigorta ücretlerini tahmin etmektir. Çalışma, Python programlama dili ve veri bilimi kütüphaneleri kullanılarak Jupyter Notebook ortamında geliştirilmiştir.

## 🔍 Proje Amacı

Sigorta şirketleri için bireylerin sigorta primlerini doğru tahmin edebilmek hem finansal planlama hem de risk yönetimi açısından kritiktir. Bu projede, regresyon modelleri yardımıyla bireylerin özelliklerinden yola çıkarak sigorta ücretlerini tahmin etmek hedeflenmiştir.

## 🧰 Kullanılan Teknolojiler

- Python 3.x
- Jupyter Notebook
- Pandas
- Numpy
- Matplotlib & Seaborn
- Scikit-learn

## 📁 Veri Kümesi

Proje kapsamında kullanılan veri kümesi, ABD merkezli bireylerin sağlık sigortası verilerini içermektedir. Veri setinde aşağıdaki sütunlar yer almaktadır:

| Sütun Adı | Açıklama |
| --------- | -------- |
| `age` | Kişinin yaşı |
| `sex` | Cinsiyet |
| `bmi` | Vücut kitle indeksi |
| `children` | Sahip olunan çocuk sayısı |
| `smoker` | Sigara içme durumu |
| `region` | Yaşanılan bölge |
| `charges` | Yıllık sigorta ücreti (hedef değişken) |

## 🧪 Uygulanan Adımlar

1. **Veri Analizi ve Görselleştirme**
   - Temel istatistiksel analizler
   - Kayıp veri kontrolü
   - Korelasyon analizi
   - Görselleştirme (Dağılım grafikleri, kutu grafikleri, ısı haritası)

2. **Veri Ön İşleme**
   - Kategorik değişkenlerin sayısal hale getirilmesi (One-Hot Encoding / Label Encoding)
   - Gerekli sütunların seçimi
   - Veri setinin eğitim/test olarak bölünmesi

3. **Modelleme ve Tahmin**
   - Lineer Regresyon
   - Karar Ağacı (Decision Tree)
   - Rastgele Orman (Random Forest)
   - Model başarılarının karşılaştırılması (R², MSE, RMSE)

4. **Sonuçların Yorumlanması**
   - Hangi değişkenlerin sigorta ücretlerini daha fazla etkilediği
   - Hangi modelin en yüksek başarıyı gösterdiği

## 📈 Model Performansları

Aşağıda test verileri üzerinden elde edilen bazı model sonuçları yer almaktadır:

| Model | R² Skoru | RMSE |
|-------|----------|------|
| Linear Regression | 0.76 | 6062.06 |
| Decision Tree | 0.84 | 4786.32 |
| Random Forest | 0.86 | 4431.85 |

> 📌 **Not:** Random Forest modeli, en düşük hata oranı ve en yüksek doğrulukla en başarılı model olarak belirlenmiştir.

## 📝 Sonuç

Bu projede çeşitli makine öğrenmesi algoritmaları ile sigorta ücreti tahminlemesi yapılmıştır. Random Forest algoritması, karmaşık veri yapısını en iyi öğrenen model olarak öne çıkmıştır. Gerçek hayat uygulamalarında, bu tür modellerin sigorta şirketlerine büyük fayda sağlayabileceği görülmektedir.

## 🚀 Çalıştırmak için

Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

```bash
git clone https://github.com/kullanici-adi/sigorta-ucret-tahmini.git
cd sigorta-ucret-tahmini
pip install -r requirements.txt
jupyter notebook SigortaÜcretTahmini.ipynb
