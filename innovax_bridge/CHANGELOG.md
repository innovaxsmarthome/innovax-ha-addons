# Değişiklikler

## 0.7.0

- Hava tahmini: panelin hava tahmini kartı günlük ve saatlik tahmini Home Assistant'tan okur.
- Takvim: takvim kartı seçili Home Assistant takvimlerinin önümüzdeki 7 günlük etkinliklerini gösterir.
- Yapılacaklar: yapılacaklar / alışveriş listesi kartı maddeleri okur; panelden madde eklenir ve tamamlandı olarak işaretlenir.
- Harita: kişi ve cihaz takipçilerinin konumu (enlem, boylam) panelin harita kartına iletilir.

## 0.6.0

- Kapı, pencere ve hareket sensörleri: sensör kapalıdan açığa geçince (hareket algılayınca) Innovax'a bildirilir. Ev yöneticisi panelde Hesap › Bildirimler › "Kapı, pencere ve hareket" kartından sensör başına "Alarm kuruluyken" ya da "Her zaman" seçerse acil durum bildirimi gider.
- Olayla birlikte evdeki alarm panelinin kurulu olup olmadığı da gönderilir ("Alarm kuruluyken" kuralı için).
- Aynı sensör en fazla 2 dakikada bir bildirilir (hareket sensörleri sık tetiklenir).

## 0.5.0

- Son Aktiviteler: panel, otomasyon, Home Assistant uygulaması ve cihazın kendisinden yapılan değişiklikler Home Assistant olay kaydından okunur.

## 0.4.0

- Canlı kamera görüntüsü (WebRTC, Home Assistant go2rtc üzerinden).

## 0.3.0

- Home Assistant içinde Innovax paneli (yan menü), çoklu eşleştirme kodu ve birden fazla mekân desteği.

## 0.2.1

- Kritik olaylar lisans durumundan bağımsız bildirilir.

## 0.2.0

- Duman, gaz, karbonmonoksit, su kaçağı ve alarm olayları Innovax'a bildirilir; internet yoksa 10 dakikaya kadar bekletilip yeniden denenir.
