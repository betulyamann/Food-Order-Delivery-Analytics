# 🚴‍♂️ Food Delivery & Logistics Analytics Engine

![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=Databricks&logoColor=white)
![Spark SQL](https://img.shields.io/badge/Spark_SQL-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

Bu proje, 100.000'den fazla yemek siparişi ve teslimat verisini içeren uçtan uca (End-to-End) bir veri analitiği mimarisidir. Ham veri **Databricks (Delta Lake & Spark SQL)** üzerinde işlenmiş, veritabanı seviyesinde temizlenmiş ve **Power BI** ile etkileşimli panolara (dashboard) dönüştürülmüştür.

---

## 📌 Proje Mimarisi

1. **Data Ingestion (Veri Yükleme):** Ham `.csv` verisi Databricks platformuna aktarıldı.
2. **Data Modeling & Transformation (SQL View Katmanı):** 
   - Metin formatındaki tarihler `TIMESTAMP` tipine dönüştürüldü.
   - İptal edilen siparişlerin teslimat sürelerinin ortalama metrikleri bozmaması için `CASE WHEN` mantığı ile veri temizliği sağlandı.
   - Sayısal metriklerin veri tipleri optimize edildi.
3. **Data Visualization (Power BI):** Hazırlanan analitik SQL View, Power BI'a aktarılarak dinamik raporlama mimarisi (Star Schema mantığı) kurgulandı.

---

## 🛠️ Kullanılan Teknolojiler

- **Veri Depolama & İşleme:** Databricks, Delta Lake
- **Sorgulama Dili:** Spark SQL / Databricks SQL
- **İş Zekası & Görselleştirme:** Power BI Desktop

---

