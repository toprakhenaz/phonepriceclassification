### Phone Price Classification Projesi:  
**Destek Vektör Makineleri ile Telefon Fiyat Sınıflandırması**

Bu projede, telefon fiyatlarını sınıflandırmak amacıyla Destek Vektör Makineleri (SVM) kullanılmıştır. Proje, üç temel bileşenden oluşmaktadır:

- **Kod:**  
  Uygulamanın tüm kodları, düzenli bir biçimde *ipnby* dosyasında yer almaktadır.

- **Veri Seti:**  
  Telefon fiyatlandırma verileri, *data* klasörü içerisinde sunulmaktadır.

- **Proje Raporu:**  
  Proje sürecini, yapılan analizleri ve elde edilen sonuçları detaylı bir şekilde açıklayan rapor, *rapor* klasöründe bulunmaktadır.

---

### Model Seçimi ve Performans Değerlendirmesi

#### En İyi Parametreler
- **Parametreler:**  
  `{'C': 10, 'degree': 2, 'gamma': 'scale', 'kernel': 'linear'}`

#### Çapraz Doğrulama (Cross-Validation) Sonuçları
- **Skorlar:**  
  `[0.93125, 0.9375, 0.921875, 0.9125, 0.93125]`
- **Ortalama CV Skoru:**  
  `0.926875`

#### Test Seti Performansı (En İyi Parametrelerle)
- **Doğruluk (Accuracy):**  
  `0.9425`
- **Sınıflandırma Raporu:**

  ```
                 precision    recall  f1-score   support

             0       0.97      0.98      0.98       105
             1       0.92      0.93      0.93        91
             2       0.90      0.90      0.90        92
             3       0.96      0.95      0.95       112

      accuracy                           0.94       400
     macro avg       0.94      0.94      0.94       400
  weighted avg       0.94      0.94      0.94       400
  ```

Bu sonuçlar, modelin telefon fiyatlarını yüksek doğrulukla sınıflandırabildiğini göstermekte olup, seçilen parametrelerin ve yapılan çapraz doğrulama çalışmalarının ne kadar etkili olduğunu ortaya koymaktadır. Projenin her bileşeni, hem teknik detayların hem de elde edilen performansın net bir şekilde anlaşılmasını sağlamaktadır.
