# Innovax Bridge

Innovax Bridge, Home Assistant'ınızı Innovax Akıllı Ev / Akıllı Ofis paneline güvenle bağlar. Yalnızca dışarı doğru bağlanır; port açmaz, uzun ömürlü token istemez.

## Mekân ekleme

1. Innovax panelinde **Bağlantılar → Home Assistant (Local Bridge) ile Bağlan → Eşleştirme kodu al**.
2. Home Assistant yan menüsünde **Innovax** paneline girin, kodu **Mekân ekle** kartına yazıp **Eşleştir**'e basın.
3. Mekân kartı birkaç saniye içinde **Çevrimiçi** olur.

Kod 10 dakika geçerlidir; süre dolarsa panelden yeni kod alın.

## Birden fazla mekân (ev + ofis)

Aynı Home Assistant birden fazla Innovax mekânına bağlanabilir. Her mekân için ayrı kod alıp Innovax panelinden ekleyin. Her mekân Innovax'ta yalnız kendi seçtiği cihazları görür; duman/gaz/su gibi kritik alarmlar yalnız sensörü cihaz listesine eklemiş mekânda çalar.

## Yapılandırma sekmesi (alternatif)

Kodları **Yapılandırma → Eşleştirme kodları** listesine de yazabilirsiniz (her satıra bir kod); eklentiyi yeniden başlatınca eşleşir. Kullanılmış kodlar listede kalsa da sorun olmaz.

## Kaldırma

- Innovax panelinden **Kaldır**: mekân bağlantısı tamamen silinir; Bridge o mekânı kendiliğinden bırakır.
- Home Assistant'taki Innovax panelinden **Bu Home Assistant'tan kaldır**: yalnız bu Bridge'deki kimlik silinir; Innovax'ta bağlantı "çevrimdışı" görünür.
