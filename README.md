# Proteus H-Köprüsü Devresi (Proteus #11)

🔗 [Web Siteme Bakmak İçin Tıkla](https://www.hakkiharmankaya.com/)

---

## ⚙️ H-Köprüsü Nedir?

H-köprüsü devresi, **DC motorların yönünü değiştirmek** için kullanılan bir devredir. Dört anahtarlı bir yapıya sahiptir ve motoru hem saat yönünde hem de saat yönünün tersine döndürebilir.

---

## 🧠 Çalışma Prensibi

| Durum        | Aktif Anahtarlar | Motorun Dönüş Yönü           |
|--------------|------------------|------------------------------|
| İleri        | Q1 ve Q4         | Saat yönünde                |
| Geri         | Q2 ve Q3         | Saat yönünün tersinde       |
| Durma        | Tümü OFF         | Dönme yok (veya kısa devre) |

---

## 🧰 Gerekli Malzemeler

- 4 adet **NPN veya PNP transistör** (BC547 vb.)
- 1 adet **DC motor**
- 4 adet **diyot** (gerilim koruma için)
- 4 adet **direnç**
- **5V/9V güç kaynağı**
- **Proteus** simülasyon yazılımı

---

## 🔧 Devre Tasarımı

### 1️⃣ Transistörleri Yerleştir

- Q1 ve Q3: Yukarı kollar (pozitif voltaj sağlar)
- Q2 ve Q4: Aşağı kollar (toprak bağlantısı sağlar)
- Motor, Q1–Q2 ve Q3–Q4 arasına bağlanır.

### 2️⃣ Diyotlarla Koruma

- Tüm transistörlerin **kolektör–emitör** uçlarına **ters yönlü diyotlar** eklenir.
- Bu diyotlar, motorun oluşturduğu ters gerilimlere karşı devreyi korur.

### 3️⃣ Transistörleri Sürme

- Her transistörün **baz ucuna direnç** bağla.
- Bu dirençler transistörlerin güvenli sürülmesini sağlar.

---

## 🛠 Proteus Kurulumu

1. **Proteus**’u aç.
2. `P` tuşu ile şu bileşenleri ekle:
   - Transistör (BC547 veya benzeri)
   - Diyot (1N4007 vb.)
   - DC motor
   - Direnç (330Ω-1kΩ arası)
   - Güç kaynağı
3. Bağlantıları yukarıdaki prensibe göre kur.

---

## ▶️ Simülasyonu Başlat

- Simülasyonda anahtarları değiştirerek motorun yönünü test et.
- Örneğin Q1 ve Q4 ON olduğunda, motor saat yönünde dönecektir.
- Q2 ve Q3 ON olduğunda motor ters yönde döner.

---

## 🎯 Uygulama Alanları

- **Robotik**: Tekerlekli robotlarda yön kontrolü
- **Otomasyon**: Küçük motor sürme sistemleri
- **Arduino projeleri**: PWM ile hız ve yön kontrolü

---

Bu projeyle hem **H-köprüsü mantığını** hem de **DC motor kontrolünü** simüle ederek öğrenmiş olacaksın.

🔗 [Web Siteme Bakmak İçin Tıkla](https://www.hakkiharmankaya.com/)
