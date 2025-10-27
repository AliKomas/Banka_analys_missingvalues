USA Bank Financial Data — Data Cleaning & Preprocessing  
Finansal Veri Temizleme (Data Cleaning) Çalışması  

Bu proje, **Kaggle üzerindeki [USA Bank Financial Data](https://www.kaggle.com/datasets/vishalsinghsangral/usa-bank-financial-data)** veri seti üzerinde yapılan **veri temizleme (data cleaning)** ve **ön işleme (preprocessing)** çalışmasını içerir.  
Amaç, verideki **eksik değerleri (missing values)** doldurmak, **tarihsel bilgileri ayrıştırmak**, veri tiplerini düzenlemek ve **finansal analiz / EDA (Exploratory Data Analysis)** için uygun hale getirmektir.  

---

Veri Seti Hakkında

Veri Seti Adı:`USA Bank Financial Data`  
Kaynak: [Kaggle – USA Bank Financial Data](https://www.kaggle.com/datasets/vishalsinghsangral/usa-bank-financial-data)  

Sütunlar:
- `Interest_Income` → Bankanın faiz gelirleri  
- `Interest_Expense` → Bankanın faiz giderleri  
- `Average_Earning_Assets` → Ortalama gelir getiren varlıklar  
- `Net_Income` → Net gelir (kar/zarar)  
- `Total_Assets` → Toplam varlıklar  
- `Shareholder_Equity` → Özsermaye  
- `Operating_Expenses` → Faaliyet giderleri  
- `Operating_Income` → Faaliyet gelirleri  
- `Market_Share` → Pazar payı (%)  
- `Stock_Price` → Hisse senedi fiyatı  
- `Year`, `Month`, `Day` → Tarih bileşenleri  

---

 Amaç

Bu notebook’un temel hedefleri:
- Eksik değerleri (NaN) ortalama (mean) yöntemiyle doldurmak  
- Sayısal değişkenleri uygun veri tipine dönüştürmek (`int`, `float`)  
- Tarih sütununu parçalayıp (`Year`, `Month`, `Day`) analiz için düzenlemek  
- Gereksiz sütunları kaldırmak  
- Veriyi finansal analiz ve modelleme (örneğin kârlılık tahmini) için hazır hale getirmek  

---

Öneri

-Aykırı Değer (Outlier) Analizi – IQR yöntemiyle tespit ve winsorizing uygulanabilir
-Korelasyon Analizi – Gelir, gider, kar ve hisse fiyatı ilişkisi incelenebilir
-Zaman Serisi Analizi – Yıllık kâr, hisse fiyatı veya varlık trendleri
-Tahminleme (Forecasting) – Stock_Price veya Net_Income tahmini
