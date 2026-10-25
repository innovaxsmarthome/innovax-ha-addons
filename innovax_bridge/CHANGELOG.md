# Değişiklikler

## 0.9.2

- Bulut komut kanalı bir kesintiden sonra kendiliğinden açılmazsa 90 saniye içinde güncel oturumla yeniden kurulur; panel komutlarının "Bridge zamanında yanıt vermedi" hatasında takılı kalması için eklentiyi yeniden başlatmak gerekmez.

## 0.9.1

- Güvenlik: Innovax panelinde eşleştirme kodu ekleme yalnız JSON isteğiyle kabul edilir; başka bir siteden form gönderimiyle kod eklenemez.
- Innovax paneli açılışta hemen açılır; seçeneklerdeki eşleştirme kodları arkadan eşleşir (yavaş ağda panel beklemez).
- Panel portu doluysa eklenti düşmez, hata loglanır.
- Kaldırılan mekânın bulut oturumu arka planda yenilenmeye devam etmez.
- Bulut yeni bir mekân türü gönderse de heartbeat çalışmaya devam eder.
- 0.2.x'ten taşıma sırasında artakalan eski kimlik dosyası (`credentials.json`) açılışta silinir.

## 0.9.0

- Otomasyon ve sahneler: Innovax panelinden kurulan otomasyonlar ve sahneler Home Assistant'a kaydedilir, açılıp kapatılır, çalıştırılır ve silinir. Innovax yalnızca kendi oluşturduğu kayıtlara dokunur.
- Bildir eylemi: otomasyon "bildir" adımına geldiğinde ev yöneticilerine Innovax bildirimi gider (sessiz saat kuralları geçerlidir).
- Home Assistant bir otomasyon ya da sahne kaydını reddederse (ör. eski sürüm yeni sözdizimini tanımaz) panel bunu ayrı bir hata olarak (`ha_rejected`) gösterir.

## 0.8.0

- Nemlendirici: hedef nem, kip ve aç/kapa panelden yönetilir; ölçülen nem gösterilir.
- Medya oynatıcı: çalan parça, oynat/duraklat, önceki/sonraki, ses düzeyi ve sessiz.
- Alarm paneli: panelden kurma (evde, dışarıda, gece, tatil) ve devre dışı bırakma. Home Assistant alarmı kod istiyorsa kod her seferinde girilir; Innovax kodu saklamaz.
- Bitki: nem, sıcaklık, iletkenlik, ışık ve pil ölçümleri ile bakım uyarısı.

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
