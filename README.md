
# Yapay Zekaya Trex Runner Oynatmak


Bu proje, "T-Rex Runner" adlı tarayıcı oyununu otomatik olarak oynamak ve yapay zeka modeli kullanarak oyunun en iyi hareketlerini tahmin etmek için geliştirilmiştir. Aynı zamanda, gerçek zamanlı olarak ekran görüntüsü kaydetmek ve bu kayıtları kullanarak modeli eğitmek için de kullanılır.

## Kullanım

Bu projeyi kullanmak için aşağıdaki adımları takip edebilirsiniz:

1. **Gereksinimler**
   - Projeyi çalıştırmak için aşağıdaki Python kütüphanelerine ihtiyaç vardır:
     - `keyboard`
     - `numpy`
     - `PIL` (Python Imaging Library)
     - `mss` (Python Screen Capture)
     - `keras` (Eğer yapay zeka modelini kullanıyorsanız)
   - Gereksinimleri yüklemek için terminale `pip install <kütüphane_adı>` komutunu kullanabilirsiniz.

2. **Veri Toplama ve Eğitim**
   - `T-Rex Runner` oyununu açın ve oyunun başladığı pencereyi tarayıcınızda belirli bir konum ve boyutta ayarlayın.
   - Proje klasöründe `record_screen.py` adlı dosyayı çalıştırarak oyun sırasında eğitim verilerini toplayın. `up`, `down` ve `right` tuşlarına basarak ekran görüntüsü kaydedebilirsiniz.
   - Kaydedilen verileri kullanarak yapay zeka modelini eğitin (`train_model.py`).

3. **Otomatik Oyun Oynama**
   - Eğitilmiş modeli kullanarak oyunu otomatik olarak oynamak için `play_game.py` dosyasını çalıştırın. Model, ekran görüntüsünden en iyi hamleleri tahmin edecektir.
   - Oyun sırasında bazı parametreleri (örneğin, gecikme süresi) ayarlayabilirsiniz.

## Dikkat

- Bu kod, oyununuzu otomatik olarak oynamak için tasarlanmıştır. Ancak bu tür otomasyonun oyunun sağlayıcıları veya hükümleri ile uyumlu olup olmadığını kontrol etmek önemlidir. Kullanım koşullarını ihlal etmemeye dikkat edin.
- Eğitilmiş yapay zeka modeli (`model_new.json` ve `trex_weight.h5`) olmadan oyunu otomatik olarak oynatmanın anlamı yoktur. Bu modeli oluşturmak ve eğitmek için veri toplama adımlarını izleyin.



## Bağımlılıkların Kurulumu

Projenin düzgün çalışabilmesi için aşağıdaki Python bağımlılıklarını kurmanız gerekmektedir. Bu bağımlılıkları `pip` komutuyla yükleyebilirsiniz.

- **keyboard**: Klavye etkileşimleri için kullanılır.

- **numpy**: Sayısal işlemler için kullanılır.

- **PIL**: Resim işleme işlemleri için kullanılır.

- **mss**: Ekran görüntüsü yakalamak için kullanılır.

- **keras**: Yapay zeka modeli eğitiminde kullanılır (sadece ilgili bölüm için gereklidir).

Bağımlılıkları yüklemek için yukarıdaki komutları kullanarak, projeyi sorunsuz bir şekilde çalıştırabilirsiniz. Ayrıca, projenizi çalıştırmadan önce Python'unuzun güncel olduğundan emin olun.


## Daha fazla Proje için [Web Sitemi Ziyaret edin](https://ayazaktas.netlify.app)


## Lisans

Bu proje özgürce kullanılabilir ve değiştirilebilir. Ancak, projenin orijinal kaynakçalarını belirtmeyi unutmayın.
