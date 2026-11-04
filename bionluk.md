# Bionluk profili — kopyala-yapıştır

Her blok doğrudan yapıştırılacak şekilde yazıldı. Sıra önemli:
Başlık → Hakkımda → Yetenekler → Portfolyo → İlanlar.

Fiyatlar TL. **1 USD = 50 TL** — kur değiştiyse çarpanı güncelle.
Bionluk komisyon kesiyor; rakamlar onu hesaba katarak belirlendi, indirme.

---

## 1. Profil başlığı

```
Steam'de oyun çıkarmış geliştirici | Oyun · Python Otomasyon · API
```

Bu başlık işe yarıyor çünkü Bionluk'ta "Python geliştirici" yüzlerce kişi,
"Steam'de oyun çıkarmış" birkaç kişi. Önce ayrış, sonra sat.

---

## 2. Hakkımda

### Kısa sürüm (alan darsa)

```
Steam'de yayınlanan bir korku oyununun geliştiricisiyim: False Signal
(Veilward Studios). Oynanışından seslendirme altyapısına, mağaza
sayfasından build sürecine kadar her şeyi kendim yaptım.

Oyun dışında: Python otomasyonu, FastAPI ile API, web scraping ve
bağımlılıksız JavaScript. GitHub'da 21 açık kaynak proje, 300'ün
üzerinde test, hepsi CI'da koşuyor.

Her teslimde üç şey veriyorum: çalışan kod, testler ve teknik bilgisi
olmayan birinin de çalıştırabileceği bir talimat. Teslimden sonra 14 gün
ücretsiz hata düzeltme.

Steam: https://store.steampowered.com/app/5353340/False_Signal/
GitHub: https://github.com/antonidashaci
```

### Uzun sürüm

```
Merhaba, ben Emre.

BİTMİŞ İŞ

Steam'de yayınlanan bir korku oyunum var: False Signal, Veilward Studios.
Birinci şahıs bir teşhis oyunu — beş mürettebattan biri artık kayıtlarına
uymuyor; oyuncu hava örneği, görev kartı ve telsiz kaydını birlikte okuyup
taşıyıcıyı buluyor. Türkçe ve İngilizce, metin ve seslendirme, tam kumanda
desteği, erişilebilirlik ayarları.

Oynanış kodu, çok dilli altyapı, ses sistemi, menüler, Steam mağaza
sayfası ve build/depot süreci: hepsi bana ait. Bir oyunu baştan sona
mağazaya çıkarmış biriyim.

https://store.steampowered.com/app/5353340/False_Signal/

NE YAPIYORUM

• Oyun: Unreal (C++/Blueprint), Unity (C#). Sistem yazımı, çok dil,
  kumanda, performans, Steamworks ve yayına çıkış.
• Otomasyon: Elle yaptığınız tekrar eden işi yapan Python programı.
  Excel/CSV birleştirme, dosya düzenleme, zamanlanmış görevler.
• Veri çekme: Siteden veri çekip Excel veya veritabanına aktarma.
• API: FastAPI ile servis yazma, hazır servislere (ödeme, kargo, SMS)
  bağlanma.
• Web: Bağımlılıksız JavaScript bileşenleri ve sayfa hızı.

NASIL ÇALIŞIYORUM

• Önce ne kırılacağını soruyorum. 21 projemde 300'ün üzerinde test var ve
  testler kolay olanı değil, kırılanı kapsıyor: saat dilimi, yuvarlama,
  Türkçe karakter, zaman aşımı, boş girdi.
• Bağımlılık hak etmeli. 21 projenin 17'sinde sıfır dış bağımlılık var.
• Teslim = çalışan kod + testler + çalıştırma talimatı. Üçü de olmadan
  teslim demiyorum.
• Teslimden sonra 14 gün ücretsiz hata düzeltme.

ÖRNEK AÇIK KAYNAK İŞLER (indirip çalıştırabilirsiniz)

• webhook-inspector — Webhook'ları yakala, oku, localhost'a birebir
  yeniden gönder. Ödeme entegrasyonunda şart.
• url-shortener-api — FastAPI + SQLite. Tahmin edilemez slug, açık
  yönlendirme koruması, süre dolumu, tıklama sayımı.
• sitemapper — Siteyi tarar, geçerli sitemap.xml üretir.
• logstats — nginx log'unu okunabilir rapora çevirir, .gz okur.
• secretscan — Commit'e sızan API anahtarlarını yakalar.
• slugify-tr, money-fmt — Türkçe karakter ve kuruş hatalarını çözer.

Tamamı: https://github.com/antonidashaci

ÇALIŞMA ŞEKLİ

Türkçe ve İngilizce. Europe/Istanbul (UTC+3). Mesajlara genelde 1 saat
içinde dönüyorum. İşe başlamadan önce ne teslim edeceğimi maddeler
halinde yazıyorum; sonradan "bu da dahil mi" tartışması olmuyor.
```

---

## 3. Yetenekler

İlk 10'u aramada en çok karşılığı olanlar — sırayı bozma:

```
Oyun Geliştirme
Unity
Unreal Engine
Python
Otomasyon
Web Scraping
API Geliştirme
FastAPI
JavaScript
Veri Analizi
C#
C++
Steam
SQLite
REST API
Excel / CSV
Bot Geliştirme
Unit Test
HTML/CSS
Teknik Dokümantasyon
```

---

## 4. Portfolyo

Her girişe görsel koy — görselsiz portfolyo tıklanmıyor. Oyun için Steam
sayfasındaki ekran görüntülerini kullan.

| Başlık | Açıklama | Link |
|---|---|---|
| **False Signal — Steam'de yayınlanan korku oyunu** | Birinci şahıs teşhis oyunu. Beş mürettebattan biri kayıtlarına uymuyor; hava örneği, görev kartı ve telsiz kaydıyla taşıyıcıyı buluyorsunuz. Her yanlış karar bir mürettebatın hayatına mal oluyor. Oynanış, çok dilli seslendirme, menüler, Steam mağaza sayfası ve build süreci: tamamı bana ait. | https://store.steampowered.com/app/5353340/False_Signal/ |
| Webhook Inspector | Gelen webhook'ları yakalar, içeriğini gösterir ve localhost'a imza başlığıyla birebir yeniden gönderir. Ödeme entegrasyonunu test ederken şart. | https://github.com/antonidashaci/webhook-inspector |
| URL Kısaltma API'si | FastAPI + SQLite, tek dosya. Tahmin edilemez slug, açık yönlendirme koruması, süre dolumu, tıklama sayımı. | https://github.com/antonidashaci/url-shortener-api |
| Sitemapper | Siteyi tarar, geçerli sitemap.xml üretir. robots.txt'ye uyar, canonical'ı anlar, aynı sayfayı beş yazımla listelemez. | https://github.com/antonidashaci/sitemapper |
| JWT Peek | JWT'yi tarayıcıda, çevrimdışı çözümleyen ve imzasını doğrulayan araç. Token'ın kendi algoritmasını seçmesine izin vermez. | https://antonidashaci.github.io/jwt-peek/ |
| Fatura Oluşturucu | Tarayıcıda fatura hazırla, PDF kaydet. KDV oran bazında gruplanır, kuruş kaymaz. | https://antonidashaci.github.io/invoice-maker/ |
| Masraf Paylaştırıcı | Ortak hesabı, kapatan en az sayıda transfere böler. | https://antonidashaci.github.io/expense-splitter/ |
| Palette Lab | Renk skalası üretir, hangi tonun üstüne yazı konabileceğini WCAG'a göre söyler. | https://antonidashaci.github.io/palette-lab/ |
| Markdown Notlar | Yerel çalışan not uygulaması; markdown çevirici sıfırdan yazıldı, XSS'e kurgusuyla kapalı. | https://antonidashaci.github.io/markdown-notes/ |

---

## 5. İlanlar

**Önce 1, 2 ve 3'ü yayınla.** İki hafta sonra kalanları ekle. Her ilana
görsel şart: oyun ekran görüntüsü, terminal çıktısı ya da Excel
öncesi/sonrası.

---

### İlan 1 — Oyun geliştirme (en ayrıştırıcı ilan, ilk bunu aç)

**Başlık:** `Unity ve Unreal ile oyun geliştirme, Steam'de yayına hazırlama`

```
Steam'de yayınlanan bir oyunun geliştiricisiyim: False Signal, Veilward
Studios. Oynanışından mağaza sayfasına kadar hepsini kendim yaptım.
Sizin oyununuzu da yazarım ya da yarıda kalmış projenizi yayınlanabilir
hale getiririm.

Yaptıklarım:
• Oynanış sistemleri — Unity'de C#, Unreal'da C++/Blueprint
• Düşman yapay zekâsı, etkileşim, envanter, kayıt/yükleme, ayarlar menüsü
• Çok dilli metin ve seslendirme altyapısı (Türkçe/İngilizce)
• Kumanda desteği ve erişilebilirlik: altyazı, FOV, titreşim, flaş uyarısı
• Performans: kare düşüşünün nereden geldiğini profiler'la bulup düzeltme
• Steam tarafı: Steamworks entegrasyonu, mağaza sayfası, build yükleme,
  depot ve beta branch kurulumu, çıkış kontrol listesi

Yarıda kalmış projeyi de alıyorum. Önce kodu inceleyip "şu durumda, şu
kadar sürer" diye yazılı bir rapor veriyorum — bu ücretsiz.

Oyunu görün: https://store.steampowered.com/app/5353340/False_Signal/
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek sistem (envanter, kayıt, menü, etkileşim) + test sahnesi | 7.500 TL | 3 gün |
| Standart | Birden çok sistem + çok dil + kumanda ve ayarlar menüsü | 25.000 TL | 8 gün |
| Premium | + Steamworks entegrasyonu, mağaza sayfası, yayına çıkış | 50.000 TL | 14 gün |

---

### İlan 2 — Python otomasyon (en çok satan kalem)

**Başlık:** `Python ile otomasyon: Excel, dosya ve rapor işlerinizi otomatikleştiriyorum`

```
Her gün elle yaptığınız işi yapan bir program yazıyorum. Tek seferlik
ödüyorsunuz, her ay kazanıyorsunuz.

Tipik işler:
• Yüzlerce Excel/CSV dosyasını birleştirip tek rapora çevirmek
• Klasördeki dosyaları adlandırma, taşıma, ayıklama, tekrarları bulma
• Bir siteden düzenli veri çekip tabloya yazmak
• Her gün saat X'te kendiliğinden çalışıp sonucu e-posta ya da
  Telegram ile göndermek
• İki dosyayı karşılaştırıp farkı raporlamak

Teslim ettiğim şey koddan ibaret değil:
• Kaynak kod — okunabilir ve yorumlu
• Çalıştırma talimatı — teknik bilgisi olmayan biri de çalıştırabilir
• Testler — kod bozulursa haber veren kontrol
• 14 gün ücretsiz hata düzeltme

İşi almadan önce: bana bir örnek dosya gönderin, ücretsiz olarak ne
kadar süreceğini ve neyi otomatikleştirebileceğimi yazayım.

Açık kaynak işlerim: csvpeek, dupefind, logstats
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek görevi yapan script + çalıştırma talimatı | 3.000 TL | 2 gün |
| Standart | Çoklu dosya/kaynak, hata yönetimi, loglama, testler | 9.000 TL | 4 gün |
| Premium | + Zamanlanmış çalışma, e-posta/Telegram bildirimi, ayar dosyası | 20.000 TL | 7 gün |

---

### İlan 3 — Web scraping

**Başlık:** `Web scraping: siteden veri çekip Excel veya veritabanına aktarma`

```
İhtiyacınız olan veriyi siteden çekip Excel, CSV ya da veritabanına
aktarıyorum.

Neyi hallediyorum:
• Sayfalama, sonsuz kaydırma, filtreli listeler
• JavaScript ile yüklenen içerik
• İstek hızını siteyi zorlamayacak şekilde sınırlama
• Çökme durumunda kaldığı yerden devam — baştan başlamaz
• Tekrar eden kayıtların ayıklanması
• Fiyat/stok takibi: değişince haber veren sürüm

Yasal not: Sadece halka açık veriyi, sitenin robots.txt kurallarına ve
kullanım şartlarına uygun şekilde çekiyorum. Giriş gerektiren ya da
kişisel veri içeren talepleri almıyorum.

Açık kaynak işim: sitemapper — siteyi tarar, sitemap.xml üretir,
robots.txt'ye uyar, canonical etiketini anlar.
github.com/antonidashaci/sitemapper
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek sayfa tipi, 1000 kayıta kadar, CSV çıktı | 4.000 TL | 2 gün |
| Standart | Sayfalama + filtreler, Excel/CSV, tekrar ayıklama | 12.500 TL | 5 gün |
| Premium | + Zamanlanmış tekrar çalışma, veritabanı, değişiklik bildirimi | 25.000 TL | 8 gün |

---

### İlan 4 — REST API ve entegrasyon

**Başlık:** `Python FastAPI ile REST API geliştirme ve servis entegrasyonu`

```
Uygulamanızın ihtiyacı olan API'yi yazıyorum ya da hazır bir servise
(İyzico, Stripe, kargo, SMS, muhasebe) bağlantısını kuruyorum.

İçerik:
• Uç nokta tasarımı ve otomatik Swagger dokümantasyonu
• Girdi doğrulama — hatalı istek hangi alanın yanlış olduğunu söyler
• Kimlik doğrulama (JWT veya API anahtarı)
• Veritabanı (SQLite veya PostgreSQL)
• Webhook alma ve imza doğrulama
• Testler ve çalıştırma talimatı

Entegrasyonlarda en sık gördüğüm dört açık, dördüne de bakıyorum: açık
yönlendirme, numarası tahmin edilebilen kayıt kimlikleri, imzası
doğrulanmamış webhook, token'ın kendi algoritmasını seçmesi.

Açık kaynak işlerim: url-shortener-api, webhook-inspector, jwt-peek
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | 3 uç noktaya kadar, doğrulama + test | 7.500 TL | 3 gün |
| Standart | 10 uç nokta, kimlik doğrulama, veritabanı, Swagger | 22.500 TL | 7 gün |
| Premium | + Webhook alma/imza doğrulama, Docker, CI | 45.000 TL | 12 gün |

---

### İlan 5 — Bot ve Discord/Telegram otomasyonu

**Başlık:** `Telegram ve Discord botu geliştirme, bildirim ve takip botları`

```
Botunuzu yazıyorum: Telegram, Discord ya da kendi panelinizle çalışan.

Tipik işler:
• Fiyat, stok, kur, duyuru takibi — değişince mesaj atan bot
• Formdan gelen veriyi tabloya yazıp ilgili kişiye bildiren akış
• Discord sunucu yönetimi: rol verme, hoş geldin, moderasyon, kayıt
• Sipariş/kargo durumunu müşteriye otomatik bildiren bot
• Yönetici komutlarıyla açılıp kapanan, ayarı dosyadan okunan yapı

Teslim: kaynak kod, sunucuya kurulum talimatı, 7/24 çalışması için
servis ayarı, testler, 14 gün ücretsiz hata düzeltme.

Not: Bir platformun kullanım şartlarını ihlal eden (sahte hesap, spam,
otomatik takip/beğeni) işleri almıyorum.
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek görevli bot, 5 komuta kadar | 3.500 TL | 2 gün |
| Standart | Çoklu komut, veritabanı, zamanlanmış görev, yönetici paneli | 12.000 TL | 5 gün |
| Premium | + Sunucuya kurulum, 7/24 çalıştırma, loglama ve izleme | 22.500 TL | 8 gün |

---

### İlan 6 — Test yazma ve kod incelemesi

**Başlık:** `Mevcut Python/JavaScript projenize test yazma ve kod incelemesi`

```
Çalışan ama dokunmaya korktuğunuz bir kod tabanınız varsa: test
yazıyorum ve ne kırılmak üzere olduğunu raporluyorum.

Teslim:
• Testler — kırılanı kapsayan: saat dilimi sınırları, yuvarlama, boş
  girdi, eşzamanlı istek, zaman aşımı
• Yazılı rapor: bulunan hatalar ciddiyetine göre sıralı, her biri için
  "şu girdiyle şu olur" örneğiyle
• GitHub Actions kurulumu — testler her commit'te kendiliğinden koşsun

Güvenlik tarafına ayrıca bakıyorum: commit'e sızmış API anahtarı, SQL
enjeksiyonu, XSS, açık yönlendirme, imzasız webhook.

Düzeltmeleri de ben yapacaksam Premium paket.

Kanıt: 21 projede 300'ün üzerinde test. secretscan — commit'e sızan
anahtarları yakalayan pre-commit aracı.
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek modül, kritik yollara test + kısa rapor | 4.500 TL | 2 gün |
| Standart | Proje geneli test + inceleme raporu + CI kurulumu | 15.000 TL | 5 gün |
| Premium | + Bulunan hataların düzeltilmesi ve refactor | 32.500 TL | 9 gün |

---

### İlan 7 — Türkçe karakter, para ve tarih hataları

**Başlık:** `Türkçe karakter, para birimi ve tarih/saat hatalarını düzeltiyorum`

```
Dar bir ilan ama bu dört hata hemen her projede var ve kimse düzeltmiyor.

1. TÜRKÇE KARAKTER
'İstanbul'.toLowerCase() 8 değil 9 kod noktası üretir; istemediğiniz bir
birleşik nokta ekler. URL'de, aramada ve veritabanı karşılaştırmasında
ı/i/İ/I karışması buradan geliyor.

2. PARA VE YUVARLAMA
0.1 + 0.2 = 0.30000000000000004. Faturalar tam da bu yüzden bir kuruş
kayıyor. Parayı tam sayı kuruş olarak tutup öyle hesaplıyorum; KDV'yi
beyanname verilir gibi oran bazında grupluyorum.

3. TARİH VE SAAT DİLİMİ
Yaz saati geçişleri, UTC ile yerel saat karışması, arka plandaki sekmenin
saati şaşırması. Tik saymak yerine saati okuyan çözüm.

4. YENİDEN DENEME
Zaman aşımına uğramış bir POST aslında başarılı olmuş olabilir —
körlemesine tekrar denemek kartı iki kez çeker. Doğrusu: üstel bekleme,
tam jitter, Retry-After başlığına uyma, POST'u varsayılan olarak tekrar
denememe.

Açık kaynak kanıt: slugify-tr, money-fmt, fetch-retry-lite
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek hata sınıfı, tespit + düzeltme + test | 4.000 TL | 2 gün |
| Standart | Proje genelinde tarama, düzeltme, regresyon testleri | 12.500 TL | 4 gün |
| Premium | + Tekrarlamasını önleyen yardımcı modül ve CI kontrolü | 22.500 TL | 7 gün |

---

## 6. Profil kontrol listesi

- [ ] Profil fotoğrafı — gerçek yüz, net, iyi ışık. Logo değil.
- [ ] Kapak görseli — False Signal'den bir kare. Oyun geliştirici olduğun
      ilk bakışta görünsün.
- [ ] Başlık (bölüm 1)
- [ ] Hakkımda (bölüm 2)
- [ ] En az 15 yetenek etiketi (bölüm 3)
- [ ] Portfolyo — 9 giriş, her birinde görsel
- [ ] İlan 1, 2, 3 yayında; her birinde görsel, varsa video
- [ ] Kimlik doğrulama — rozet satış oranını belirgin artırıyor
- [ ] Mesajlara 1 saat içinde dön; yanıt süresi sıralamayı etkiliyor

---

## 7. İlk 10 iş ve teklif şablonu

İlk yorumlar her şeyi belirliyor. İlk 3 işi Temel paket fiyatının
yarısına al, karşılığında detaylı yorum iste. 10 yorumu geçince
fiyatları yukarıdaki seviyeye çek ve bir daha inme.

Teklif şablonu (uzatma, 5 satır):

```
Merhaba [isim],

[İlandan tek bir cümleye değin — okuduğunu gösterir.]

Bunu daha önce yaptım: [en yakın tek iş + link]. [Tek cümlede sonuç.]

Sizin işte şu üç adımı yapacağım: [1], [2], [3].
[X] günde teslim ederim. Başlamadan önce [şu tek soruyu] netleştirelim.
```

İki değil, bir link. Beş link atmak "ilanını okumadım" demektir.
