# 🧠 Transformer-Based Sentiment Analysis / Transformer Tabanlı Duygu Analizi

This project demonstrates how to build a sentiment analysis model using a custom Transformer-based neural network architecture.  
Bu proje, özel olarak tasarlanmış bir Transformer tabanlı sinir ağı kullanarak duygu analizi modelinin nasıl oluşturulacağını göstermektedir.

---

## 📂 Project Structure / Proje Yapısı

- `TransformerModel`: Defines the custom Transformer model.  
  `TransformerModel`: Özel Transformer modelinin tanımını içerir.

- Training: The model is trained on the IMDb movie review dataset.  
  Eğitim: Model, IMDb film yorumu veri kümesi ile eğitilmiştir.

- Visualization: Training and validation accuracy/loss graphs are plotted.  
  Görselleştirme: Eğitim ve doğrulama doğruluk/kayıp grafikleri çizilir.

- Prediction: A function is provided for predicting sentiment of custom user input.  
  Tahmin: Kullanıcının kendi girdiği yorumlar için duygu tahmini yapılmasını sağlar.

---

## 📦 Requirements / Gereksinimler

- TensorFlow  
- NumPy  
- Matplotlib  
- (Optional) Jupyter Notebook for interactive exploration  
- (İsteğe bağlı) Jupyter Notebook ile etkileşimli kullanım

Install dependencies / Gerekli kütüphaneleri yüklemek için:

```bash
pip install tensorflow numpy matplotlib
```

## 🛠️ Usage / Kullanım
1. Train the Model / Modeli Eğit
Run the notebook to build and train the model on IMDb dataset.
Notebook'u çalıştırarak modeli IMDb veri kümesinde eğitin.

2. Visualize Results / Sonuçları Görselleştir
The script will plot training and validation loss and accuracy graphs.
Eğitim ve doğrulama süreci boyunca kayıp ve doğruluk değerlerini grafik olarak gösterir.

3. Predict from Custom Input / Kullanıcı Girdisi ile Tahmin Yap
After training, the user can input a movie review and get sentiment prediction.
Eğitim tamamlandıktan sonra kullanıcı, bir film yorumu girerek duygu analiz sonucunu görebilir.

Example / Örnek:
```bash
Enter a movie review:/Film yorumu giriniz: This movie was absolutely amazing!
Predicted sentiment: Positive -> Score: 0.91 / Tahmin sonucu olumlu -> skor: 0.91(%91)
```
## 🧪 Model Details / Model Detayları
- Embedding Size / Embedding Boyutu: **64**
- Transformer Layers / Transformer Katmanı: **4**
- Attention Heads / Baş Sayısı: **4**
- Dropout Rate / Dropout Oranı: **0.3**
- Classification Type / Sınıflandırma Türü: Binary Sentiment (Positive/Negative)
Binary Duygu Analizi (Olumlu/Olumsuz)


## 📊 Output Example / Çıktı Örneği
- Training/Validation Loss Graph
 Eğitim/Doğrulama Kayıp Grafiği

- Training/Validation Accuracy Graph
 Eğitim/Doğrulama Doğruluk Grafiği


![ssss](https://github.com/user-attachments/assets/911b4fc9-e570-4c90-9d78-14b8700d5a26)



## 🚨 Overfitting Case /Overfitting Durumu 

**Our model overfitted... 🙄**

**Modelimiz overfitting yaptı... 🙄**  

The model memorized the training data but failed on validation.

Model eğitim verisini ezberledi ama doğrulama verisinde başarısız oldu.  


### 🔍 How to detect overfitting? /Overfitting nasıl anlaşılır? 

 - Very high training accuracy ✅
 - Low validation accuracy ❌
   
- Eğitim doğruluğu çok yüksek ✅  
- Doğrulama doğruluğu düşük ❌  


### 🛠️ Quick fixes / Hızlı çözümler 

- Increase `dropout_rate`
- Reduce `num_layers` or `embed_size`
- Use `early stopping`
- Add more training data
- 
- `dropout_rate` değerini artırın  
- `num_layers` veya `embed_size` değerlerini azaltın  
- `early stopping` kullanın  
- Daha fazla eğitim verisi ekleyin  
  
> 💡 Feel free to tweak these parameters to reduce overfitting.

> 💡 Dilerseniz bu parametrelerle oynayarak overfitting'i azaltabilirsiniz.  


## 👤 Author / Yazar
Developed by *Teymur Mammadov* as part of a deep learning sentiment analysis project.

Bu proje, derin öğrenme temelli duygu analizi çalışması kapsamında *Teymur Mammadov* tarafından geliştirilmiştir.


## 📜 License / Lisans
- MIT License — feel free to use and modify.
- MIT Lisansı — kullanmakta ve değiştirmekte özgürsünüz.


