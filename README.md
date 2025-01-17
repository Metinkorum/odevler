# İleri Mikroişlemci Projeleri

Bu depo, **İleri Mikroişlemciler** dersi kapsamında geliştirilen ve **Tiva C Series (TM4C123GXL)** mikrodenetleyicisi kullanılarak gerçekleştirilen projeleri içermektedir. Projeler, gömülü sistem programlamasının çeşitli özelliklerini ve yeteneklerini sergilemektedir. Geliştirme ortamı olarak **Code Composer Studio** kullanılmıştır.

---

## İçindekiler

- [Proje Açıklamaları](#proje-açıklamaları)
- [Kurulum ve Gereksinimler](#kurulum-ve-gereksinimler)
- [Nasıl Kullanılır?](#nasıl-kullanılır)
- [Lisans](#lisans)

---

## Proje Açıklamaları

### 1. LCD'ye Karakter Yazdırma
- **Amacı:** Tiva C Series mikrodenetleyicisine bağlı bir LCD'ye karakter yazdırmak.
- **Açıklama:** Bu proje, GPIO pinlerini yapılandırarak bir LCD ile iletişim kurmayı ve ASCII karakterleri ekranda göstermeyi içerir.
- **Özellikler:**
  - Özel karakterlerin gösterimi.
  - Ekranın dinamik olarak temizlenmesi ve güncellenmesi.

  ![LCD PINS](https://github.com/Metinkorum/odevler/blob/main/proje1/2x16-lcd-ekran-sol-ust-mavi-qapass__1350064996275180.jpg)

### 2. Timer Uygulaması
- **Amacı:** Yazılım tabanlı bir 24 saatlik zamanlayıcı oluşturmak.
- **Açıklama:** Bu proje, mikrodenetleyicinin dahili zamanlayıcılarını kullanarak tamamen yazılımda çalışan bir zamanlayıcı simülasyonu yapmayı hedefler.

![Timer Örnek Görsel](https://github.com/Metinkorum/odevler/blob/main/proje2/T%C4%B0MER.jpeg)

### 3. Sharp Develop ile Eşzamanlı Timer Uygulaması
- **Amacı:** Bir zamanlayıcıyı Sharp Develop ile gerçek zamanlı olarak senkronize etmek.
- **Açıklama:**
  - Sharp Develop'ta bir form üzerinden mikrodenetleyiciye başlangıç zamanı gönderilir.
  - Zamanlayıcı, LCD'de ve Sharp Develop üzerindeki bir metin kutusunda eşzamanlı olarak görüntülenir.
  - Gerçek zamanlı veri akışı sağlanır.
 
# Fom Uygulaması Görsel
![Form Tasarımı](https://github.com/Metinkorum/odevler/blob/main/proje3/form%20tasar%C4%B1m.png)

### 4. ADC ile Sıcaklık Ölçümü
- **Amacı:** ADC modülünü kullanarak bir 10k'lık potansiyometre ile sıcaklık ölçümü yapmak.
- **Açıklama:**
  - Tiva C'nin ADC modülü yapılandırılarak analog sinyaller okunur.
  - Analog sinyal, sıcaklık değerine dönüştürülür.
  - Ölçülen sıcaklık değeri LCD'de gösterilir.

### 5. Hibernasyon Modu
- **Amacı:** Güç tasarrufu sağlamak için hibernasyon modunu kullanmak.
- **Açıklama:** Bu proje, Tiva C'nin hibernasyon modülünü kullanarak güç tasarrufu tekniklerini uygular.

### 6. Floating Point İşlemleri
- **Amacı:** Ondalık sayılarla aritmetik işlemler yapmak.
- **Açıklama:** Mikrodenetleyicinin kayan nokta işlemlerini nasıl etkin bir şekilde gerçekleştirebildiğini gösterir.

---

## Kurulum ve Gereksinimler

### Donanım
- **Tiva C Series (TM4C123GXL)** mikrodenetleyicisi
- LCD modülü
- Potansiyometre (10k)
- Gerekli bağlantı kabloları ve devre tahtası

### Yazılım
- [Code Composer Studio](https://www.ti.com/tool/CCSTUDIO)
- Sharp Develop (Proje 3 için)
- Energia (isteğe bağlı ek testler için)

### Bağımlılıklar
Aşağıdaki kütüphane ve araçların kurulu olduğundan emin olun:
- TivaWare sürücü kütüphanesi.
- USB hata ayıklama için gerekli cihaz sürücüleri.

---

## Nasıl Kullanılır?

1. Depoyu klonlayın:
   ```bash
   [git clone https://github.com/kullanici-adi/ileri-mikroislemci-projeleri.git](https://github.com/Metinkorum/odevler.git)
   ```

2. İlgili projeyi **Code Composer Studio** ile açın.

3. **Tiva C Series** mikrodenetleyicinizi bilgisayarınıza bağlayın.

4. Kodu derleyin ve mikrodenetleyiciye yükleyin.

5. Her proje için belirtilen donanım bağlantılarını yapın ve talimatları takip edin.

---


