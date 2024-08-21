# R-Project

R-Project deposuna hoş geldiniz! Bu proje, Albury bölgesinden alınan hava durumu verilerini kullanarak çeşitli analizler ve görselleştirmeler yapmayı amaçlamaktadır. Projenin ana hedefi, farklı hava durumu değişkenleri arasındaki ilişkileri keşfetmek, istatistiksel testler yapmak ve bu ilişkileri zaman içinde göstermek için animasyonlu görselleştirmeler oluşturmaktır. Aynı zamanda MARS yöntemiyle makina öğrenmesine de değinmektedir.

## İçindekiler

- [Proje Hakkında](#proje-hakkında)
- [Veri](#veri)
- [Analiz](#analiz)
- [Görselleştirmeler](#görselleştirmeler)
- [Projenin Çalıştırılması](#projenin-çalıştırılması)

## Proje Hakkında

Bu proje, Albury bölgesinden alınan hava durumu verilerini analiz etmeye odaklanmaktadır. Yapılan analizler arasında:

- Değişkenler arasındaki ilişkileri keşfetmek için regresyon analizi.
- Yıllar boyunca sıcaklıklarda anlamlı farklılıklar olup olmadığını belirlemek için ANOVA testleri.
- Zaman içinde sıcaklıklardaki değişiklikleri görselleştirmek için animasyonlu grafikler.

## Veri

Bu projede kullanılan veri, Albury bölgesine ait hava durumu bilgilerini içermektedir. Anahtar değişkenler şunlardır:

- **Date**: Gözlemin yapıldığı tarih.
- **Temp3pm**: Saat 3'te kaydedilen sıcaklık.
- **MaxTemp**: Gün içinde kaydedilen maksimum sıcaklık.
- **MinTemp**: Gün içinde kaydedilen minimum sıcaklık.
- **Humidity3pm**: Saat 3'te kaydedilen nem oranı.
- **Year**: Verinin kaydedildiği yıl.

## Analiz

### Regresyon Analizi

Sıcaklık ve nem, minimum ve maksimum sıcaklıklar arasındaki ilişkileri keşfetmek için bir dizi regresyon modeli oluşturulmuştur.

### ANOVA Testi

3 PM sıcaklıklarının farklı yıllar arasında anlamlı bir fark olup olmadığını analiz etmek için ANOVA testi yapılmıştır.

### Post-hoc Testi
ANOVA sonucunda anlamlı bir fark bulunursa, Tukey's HSD testi ile hangi yıllar arasında istatistiksel olarak anlamlı farklar olduğunu belirlemek mümkündür.


## Görselleştirmeler

Bu projede, hava durumu verilerinin daha iyi anlaşılabilmesi için çeşitli görselleştirmeler oluşturulmuştur. Görselleştirmeler, veri setindeki farklı değişkenlerin zaman içindeki değişimini ve birbirleriyle olan ilişkilerini görselleştirir. Kullanılan temel araç `ggplot2` paketidir ve bu paket ile güçlü ve özelleştirilebilir grafikler üretilmiştir.

### Sıcaklık ve Nem İlişkisi

Saat 3'te kaydedilen sıcaklık ve nem oranı arasındaki ilişkiyi anlamak için bir scatter plot oluşturulmuştur. Bu grafik, sıcaklık ve nem arasındaki potansiyel doğrusal ilişkiyi görselleştirmeyi amaçlamaktadır.

### Minimum ve Maksimum Sıcaklıklar

Minimum ve maksimum sıcaklıklar arasındaki ilişkiyi göstermek için bir scatter plot kullanılmıştır. Bu grafik, sıcaklıkların günlük değişimini ve ekstrem değerlerin nasıl dağıldığını anlamaya yardımcı olur.

### Animasyonlu Sıcaklık Değişiklikleri

Sıcaklıkların zaman içindeki değişimini daha dinamik bir şekilde göstermek için `gganimate` paketi kullanılarak bir animasyon oluşturulmuştur. Bu animasyon, yıllara veya aylara göre sıcaklık değişimlerini izleyicilere görsel olarak sunar. Animasyonlu grafikler, verilerin zaman içinde nasıl değiştiğini daha etkili bir şekilde gösterebilir.

Bu görselleştirmeler, verilerin daha iyi yorumlanmasına olanak tanır ve analizlerin sonuçlarını görsel bir formatta sunarak daha anlaşılır hale getirir.

## Projenin Çalıştırılması

Bu projeyi çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

### 1. Depoyu Klonlayın

İlk olarak, projeyi kendi yerel makinenize klonlayarak başlayın. Aşağıdaki komutla projeyi klonlayabilirsiniz:

```bash
git clone https://github.com/halilkkaya/R-Project.git


 # Gerekli Kütüphaneleri Çalıştırın
install.packages(c("ggplot2", "dplyr", "gganimate", "car", "lmtest"))

# gerekli scriptleri açın ve çalıştırın





