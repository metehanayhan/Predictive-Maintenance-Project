[EN]
# Predictive Maintenance Project

## Project Overview
This project aims to develop a predictive maintenance model for a delivery company. The objective is to predict equipment failures in advance using machine learning, allowing the company to perform timely maintenance and reduce the risk of unexpected downtimes.

## Solutions and Methodology

1. **Exploratory Data Analysis (EDA):** Conducted an initial analysis of the dataset to understand the distribution of variables, identify patterns, and detect any imbalances or anomalies in the data.

2. **Data Preprocessing:** 
   - Converted the date column into separate year, month, and day columns.
   - Simplified the device identification by extracting the first letter of the device code and applying One-Hot Encoding.
   - Handled missing values and cleaned the dataset to ensure quality data for model training.

3. **Feature Engineering:** 
   - Extracted new features such as year, month, and day from the date column.
   - Applied One-Hot Encoding to categorical variables like device code to make them suitable for machine learning algorithms.

4. **Handling Imbalanced Data:** 
   - Used SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset, addressing the challenge of having a small number of failure instances compared to non-failure instances.

5. **Model Selection and Training:** 
   - Tested several classification algorithms, including Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, and Decision Tree, to identify the best-performing model.
   - The RandomForestClassifier was selected as the final model due to its high accuracy of 99.97%.

6. **Evaluation:**
   - Evaluated the model using accuracy, confusion matrix to ensure robust performance.
   - The final model demonstrated exceptional performance with an accuracy of 99.96% in predicting equipment failures.

## Dataset Description
- **date:** The date on which the data was collected.
- **device:** The unique identifier or code of the device.
- **failure:** A binary label indicating whether the device failed on the given date (0 = no failure, 1 = failure).
- **attribute1 - attribute9:** Numerical values representing various features or sensor readings of the device on the given date.

## Libraries Used
- **pandas**: Data manipulation and analysis.
- **matplotlib** & **seaborn**: Data visualization.
- **scikit-learn**: Machine learning algorithms and model evaluation.
- **imblearn (SMOTE)**: Handling imbalanced datasets.
- **warnings**: Suppressing warnings for cleaner outputs.

## Results
Using a RandomForestClassifier, a predictive maintenance model was developed with an accuracy of 99.96%. The model can effectively predict equipment failures, enabling the delivery company to take proactive measures and minimize downtime.

[TR]
# Predictive Maintenance Project

## Proje Özeti
Bu proje, bir dağıtım şirketi için predictive maintenance modeli geliştirmeyi amaçlamaktadır. Amaç, ekipman arızalarını önceden tahmin ederek zamanında bakım yapılmasını sağlamak ve beklenmeyen duruş sürelerini en aza indirmektir.

---

## Çözümler ve Yöntemler

1. **Exploratory Data Analysis (EDA):** 
   - Veri seti analiz edilerek değişkenlerin dağılımı incelendi, kalıplar tespit edildi ve dengesizlikler ya da anormallikler belirlendi.

2. **Data Preprocessing:** 
   - Tarih sütunundan yıl, ay ve gün bilgileri çıkarıldı.
   - Cihaz kodları sadeleştirilerek ilk harflerinden oluşan bir kategoriye dönüştürüldü ve One-Hot Encoding uygulandı.
   - Eksik değerler temizlendi ve yüksek kaliteli bir veri seti oluşturuldu.

3. **Feature Engineering:** 
   - Tarih sütunundan türetilen yıl, ay ve gün gibi yeni özellikler oluşturuldu.
   - Cihaz kodları gibi kategorik değişkenler, makine öğrenimi algoritmalarına uygun hale getirilmek için One-Hot Encoding ile işlendi.

4. **Handling Imbalanced Data:** 
   - Veri setindeki dengesizlikler, SMOTE (Synthetic Minority Over-sampling Technique) yöntemi kullanılarak giderildi. Böylece arıza durumları yeterince temsil edilebildi.

5. **Model Selection and Training:** 
   - Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes ve Decision Tree gibi çeşitli sınıflandırma modelleri test edildi.
   - RandomForestClassifier, %99.97 doğruluk oranıyla en iyi model olarak seçildi.

6. **Evaluation:**
   - Modelin performansı, accuracy ve confusion matrix gibi metriklerle değerlendirildi.
   - Nihai model, %99.96 doğruluk oranıyla ekipman arızalarını başarılı bir şekilde tahmin etti.

---

## Dataset Description
- **date:** Verinin toplandığı tarih.
- **device:** Cihaz kodu.
- **failure:** Cihazın belirtilen tarihte arıza yapıp yapmadığını gösteren binary bir etiket (0 = arıza yok, 1 = arıza var).
- **attribute1 - attribute9:** Cihazın o tarihteki çeşitli özelliklerini veya sensör ölçümlerini temsil eden sayısal değerler.

---

## Libraries Used
- **pandas**: Veri işleme ve analiz.
- **matplotlib** & **seaborn**: Veri görselleştirme.
- **scikit-learn**: Makine öğrenimi algoritmaları ve model değerlendirme.
- **imblearn (SMOTE):** Veri dengesizliklerini giderme.
- **warnings**: Temiz çıktı için uyarıları bastırma.

---

## Results
RandomForestClassifier kullanılarak, %99.96 doğruluk oranına sahip bir predictive maintenance modeli geliştirilmiştir. Bu model, ekipman arızalarını etkin bir şekilde tahmin ederek dağıtım şirketinin proaktif önlemler almasını ve duruş sürelerini en aza indirmesini sağlamaktadır.

