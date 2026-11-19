# Duel Legend

Android için dokunmatik kart düellosu oyunu. Hikaye modu, serbest düello, deste hazırlama ve kart listesi içerir. Tüm kartlar açıktır, kilit yoktur.

## APK indirme

1. Üstteki **Actions** sekmesine gir.
2. En son **Build APK** çalışmasını aç. Çalışmıyorsa **Run workflow** düğmesine bas.
3. Çalışma bitince sayfanın en altındaki **Artifacts** bölümünden `DuelLegend-APK` dosyasını indir.
4. Zip'i aç ve `app-debug.apk` dosyasını telefona kur. Android "bilinmeyen kaynaklardan kurulum" izni isteyebilir.

## Oynanış

- **Hikaye:** Altın Arena'da sekiz rakibi sırayla yen. Diyaloglarda devam etmek için dokun.
- **Serbest Düello:** Kendi deste ile rastgele bir rakibe karşı oyna.
- **Deste Hazırla:** Her karttan en fazla 3 kopya, deste 60 karta kadar.
- Eldeki karta dokun: Çağır, Kapalı koy veya Aktif et.
- Sahadaki canavara dokun: Saldır, Flip veya pozisyon değiştir.
- Saldırmak için önce **Savaş** düğmesine bas. İlk turda saldırı yoktur.

## Notlar

- Kart bilgileri ve görselleri ilk açılışta internetten indirilir, bu yüzden ilk açılışta internet gerekir.
- Kart verisi ve görseller [YGOPRODeck](https://ygoprodeck.com) üzerinden gelir.
- Çalışan büyüler: Pot of Greed, Dark Hole, Raigeki, Heavy Storm, Fissure, Mystical Space Typhoon, Monster Reborn, Dian Keto the Cure Master.
- Çalışan tuzaklar: Trap Hole, Mirror Force, Magic Cylinder, Negate Attack.
- Diğer kartlarda etki henüz yok, canavarlar sadece ATK/DEF ile savaşır.
- Sesler ve müzik kod ile üretilir, ses dosyası içermez.
- Hikaye karakterleri ve diyaloglar orijinaldir.

## Yapı

```
.github/workflows/build.yml                      APK derleme
app/src/main/AndroidManifest.xml
app/src/main/java/com/example/ygo/MainActivity.kt  WebView kabuğu, tam ekran
app/src/main/assets/index.html                   oyunun tamamı
```

## Bağımsız proje notu

Bu proje Konami ile bağlantılı değildir. Kart isimleri, görselleri ve oyun kuralları ilgili hak sahiplerine aittir. Kişisel ve eğitim amaçlı bir hayran projesidir.
