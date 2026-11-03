# Bionluk profili — hazır metinler

Giriş yaptıktan sonra bu dosyadaki blokları ilgili alanlara yapıştır.
Sıra: Profil Başlığı → Hakkımda → Yetenekler → Portfolyo → İlanlar (gig).

`[DEĞİŞTİR]` işaretli yerler, gerçek müşteri işlerini hatırladığında
değiştireceğin yerler. Onun dışındaki her şey gerçek GitHub projelerine
dayanıyor — uydurma referans yok.

---

## 1. Profil başlığı (Meslek / Headline)

```
Python & JavaScript Geliştirici | API, CLI, Otomasyon, Web Uygulaması
```

Alternatif (otomasyon işlerini öne çıkarmak istersen):

```
Otomasyon ve API Geliştirici | Python · FastAPI · Vanilla JS
```

---

## 2. Hakkımda

### Kısa (≈ 500 karakter — alan darsa bunu kullan)

```
Küçük ve sağlam yazılımlar yazıyorum: Python CLI araçları, FastAPI
servisleri ve bağımlılıksız JavaScript kütüphaneleri.

GitHub'da 21 açık kaynak projem var, 300'ün üzerinde testle ve CI ile.
21 projenin 17'sinde hiçbir dış bağımlılık yok — bir paketin projeye
girmesi için hak etmesi gerekiyor.

İşin asıl kırıldığı yerlere çalışıyorum: yuvarlama, para, saat dilimi,
Türkçe karakterler, zaman aşımı sonrası yeniden deneme.

Türkçe ve İngilizce. Her teslimde çalışan kod, testler ve nasıl
çalıştırılacağını anlatan bir README oluyor.

GitHub: https://github.com/antonidashaci
```

### Uzun (alan izin verirse)

```
Merhaba, ben Emre.

Küçük ve sağlam yazılımlar yazıyorum: Python CLI araçları, FastAPI
servisleri ve bağımlılıksız JavaScript kütüphaneleri. GitHub'da 21 açık
kaynak projem var — hepsi testli, hepsi CI'da koşuyor, 17'sinde hiçbir
dış bağımlılık yok.

NASIL ÇALIŞIYORUM

• Önce problem. Yazdığım her projenin README'si bir API tablosuyla değil,
  o kodun önlediği hatayla başlıyor.
• Bağımlılık hak etmeli. 21 projenin 17'sinde sıfır bağımlılık var.
  İstisnalar FastAPI ve Pillow — onları kendim yazmak saçma olurdu.
• Testler kolay olanı değil, kırılanı kapsıyor: saat dilimi sınırları,
  float kayması, vergi dairesinin yuvarlama yöntemi, XSS yükleri,
  bir saat arka planda kalmış sekme.
• Güvenlik bir filtre değil. Kodu, güvensiz durumun hiç oluşamayacağı
  şekilde sıralıyorum.

ÖRNEK İŞLER (hepsi açık kaynak, indirip çalıştırabilirsiniz)

• webhook-inspector — Gelen webhook'ları yakala, oku ve localhost'a
  birebir yeniden gönder. Stripe/GitHub entegrasyonu yaparken şart.
• url-shortener-api — FastAPI + SQLite. Tahmin edilemez slug, açık
  yönlendirme koruması, süre dolumu, tıklama sayımı.
• sitemapper — Siteyi tara, geçerli sitemap.xml üret. robots.txt'ye uyar,
  canonical etiketini anlar.
• logstats — nginx/Apache log'unu okunabilir rapora çevirir. Path başına
  p95, en çok hata, en çok istemci. .gz dosyasını doğrudan okur.
• secretscan — Commit'e sızan API anahtarlarını ve veritabanı parolalarını
  yakalar. 13 kural, üç katmanlı yanlış-pozitif filtresi.
• slugify-tr — Türkçe'ye uygun slug. 'İstanbul'.toLowerCase() 8 değil
  9 kod noktası üretir; istemediğiniz bir birleşik nokta ekler.
• money-fmt — Parayı tam sayı kuruş olarak tutar, biçimlendirir VE
  ayrıştırır. Faturalar tam da 0.1 + 0.2 yüzünden bir kuruş kayar.
• jwt-peek — JWT'yi çevrimdışı çözümle ve doğrula. Token'ın kendi
  doğrulama algoritmasını seçmesine izin vermez.

Tamamı: https://github.com/antonidashaci

ÇALIŞMA ŞEKLİ

Türkçe ve İngilizce. Saat dilimi: Europe/Istanbul (UTC+3).
Her teslimde: çalışan kod + testler + kurulum/çalıştırma README'si.
Teslimden sonra 14 gün ücretsiz hata düzeltme.
```

---

## 3. Yetenekler (etiketler)

Öncelik sırası — üstteki 10'u aramada en çok karşılığı olanlar:

```
Python
JavaScript
API Geliştirme
FastAPI
Web Scraping
Otomasyon
Veri Analizi
SQLite
REST API
HTML/CSS
Git
GitHub Actions
Web Components
Unit Test
CLI Uygulama
Excel / CSV
Bot Geliştirme
Teknik Dokümantasyon
```

---

## 4. Portfolyo girişleri

Demo linki olanların ekran görüntüsünü al; Bionluk portfolyoda görsel
istiyor.

| Başlık | Açıklama (olduğu gibi yapıştır) | Link |
|---|---|---|
| JWT Peek | JWT token'ı tarayıcıda, çevrimdışı çözümleyen ve HS256 imzasını doğrulayan araç. Token'ın kendi algoritmasını seçmesine izin vermez. | https://antonidashaci.github.io/jwt-peek/ |
| Fatura Oluşturucu | Tarayıcıda fatura hazırla, PDF olarak kaydet. KDV, beyanname verilir gibi oran bazında gruplanır. | https://antonidashaci.github.io/invoice-maker/ |
| Palette Lab | Renk skalası üretir ve hangi tonun üstüne gerçekten yazı konabileceğini WCAG'a göre söyler. | https://antonidashaci.github.io/palette-lab/ |
| Markdown Notlar | Yerel çalışan not uygulaması — markdown çevirici sıfırdan yazıldı, XSS'e filtreyle değil kurgusuyla kapalı. | https://antonidashaci.github.io/markdown-notes/ |
| Masraf Paylaştırıcı | Ortak hesabı, kapatan en az sayıda transfere böler. Tek kuruş kaybolmaz. | https://antonidashaci.github.io/expense-splitter/ |
| Pomodoro | Sekme bir saat arka planda kaldıktan sonra bile doğru. Tik saymak yerine saati okuyor. | https://antonidashaci.github.io/pomodoro-focus/ |
| webhook-inspector | Webhook'ları yakalar, içeriğini gösterir ve localhost'a imza başlığıyla birlikte birebir yeniden gönderir. | https://github.com/antonidashaci/webhook-inspector |
| sitemapper | Siteyi tarar, geçerli sitemap.xml üretir. robots.txt'ye uyar, canonical'ı anlar, aynı sayfayı beş farklı yazımla listelemez. | https://github.com/antonidashaci/sitemapper |

`[DEĞİŞTİR]` — Gerçek müşteri işlerini hatırladığında bu tablonun başına
2-3 tanesini ekle. Müşteri işi, açık kaynak projeden daha ağır basıyor.
Format: ne istendi → ne yaptın → ölçülebilir sonuç.

---

## 5. İlanlar (gig) — 6 adet

Bionluk'ta profil değil **ilanlar** iş getiriyor. Başlıklar arama
kelimesiyle başlıyor.

Fiyatlar USD; Bionluk TL istiyor — güncel kurla çevir. Taban: saatlik
20 USD, sabit işte 150 USD altına inme (ilk 5 iş hariç, bkz. bölüm 7).

---

### İlan 1 — Python otomasyon ve veri işleme

**Başlık:** `Python ile otomasyon scripti ve veri işleme yazılımı geliştirme`

```
Elle yaptığınız tekrar eden işi yapan bir Python programı yazıyorum.

Tipik işler:
• Yüzlerce Excel/CSV dosyasını birleştirip tek rapora çevirmek
• Klasördeki dosyaları adlandırma, taşıma, ayıklama, tekrarları bulma
• Bir siteden düzenli veri çekip tabloya yazmak
• Zamanlanmış görev: her gün saat X'te çalışsın, sonucu e-posta ile göndersin

Teslim edeceğim şey çalışan koddan ibaret değil:
• Kaynak kod (okunabilir, yorumlu)
• Çalıştırma talimatı — teknik bilgisi olmayan biri de çalıştırabilir
• Testler — kod bozulursa haber veren bir kontrol
• 14 gün ücretsiz hata düzeltme

Benzer açık kaynak işlerim:
csvpeek — CSV'nin sütun tiplerini, boş oranını, aralığını çıkarır
dupefind — Aynı içerikli dosyaları bulur, üç aşamalı, hiçbir şeyi silmez
logstats — nginx log'unu okunabilir rapora çevirir
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek görevi yapan script + talimat | 60 USD | 2 gün |
| Standart | Çoklu dosya/kaynak, hata yönetimi, loglama, testler | 180 USD | 4 gün |
| Premium | + Zamanlanmış çalışma, e-posta/Telegram bildirimi, ayar dosyası | 400 USD | 7 gün |

---

### İlan 2 — Web scraping

**Başlık:** `Web scraping: siteden veri çekip Excel veya veritabanına aktarma`

```
İhtiyacınız olan veriyi siteden çekip Excel, CSV veya veritabanına
aktarıyorum.

Neyi hallediyorum:
• Sayfalama, sonsuz kaydırma, filtreli listeler
• JavaScript ile yüklenen içerik
• İstek hızını siteyi zorlamayacak şekilde sınırlama
• Çökme durumunda kaldığı yerden devam — baştan başlamaz
• Tekrar eden kayıtların ayıklanması

Yasal not: Sadece halka açık veriyi, sitenin robots.txt kurallarına ve
kullanım şartlarına uygun şekilde çekiyorum. Giriş gerektiren ya da
kişisel veri içeren talepleri almıyorum.

Benzer açık kaynak işim:
sitemapper — Siteyi tarar, sitemap.xml üretir, robots.txt'ye uyar,
canonical etiketini anlar.
github.com/antonidashaci/sitemapper
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek sayfa tipi, 1000 kayıta kadar, CSV çıktı | 80 USD | 2 gün |
| Standart | Sayfalama + filtreler, Excel/CSV, tekrar ayıklama | 250 USD | 5 gün |
| Premium | + Zamanlanmış tekrar çalışma, veritabanına yazma, değişiklik bildirimi | 500 USD | 8 gün |

---

### İlan 3 — REST API geliştirme

**Başlık:** `Python FastAPI ile REST API geliştirme ve servis entegrasyonu`

```
Uygulamanızın ihtiyacı olan API'yi yazıyorum ya da hazır bir servise
(Stripe, İyzico, kargo, SMS, muhasebe) bağlantısını kuruyorum.

İçerik:
• Uç nokta tasarımı ve otomatik Swagger dokümantasyonu
• Girdi doğrulama — hatalı istek hangi alanın yanlış olduğunu söyler
• Kimlik doğrulama (JWT veya API anahtarı)
• Veritabanı (SQLite veya PostgreSQL)
• Webhook alma ve imza doğrulama
• Testler ve çalıştırma talimatı

Güvenlik tarafında en sık gördüğüm dört açık, dördüne de bakıyorum:
açık yönlendirme, numarası tahmin edilebilen kayıt kimlikleri, imzası
doğrulanmamış webhook, token'ın kendi algoritmasını seçmesi.

Benzer açık kaynak işlerim:
url-shortener-api — FastAPI + SQLite, tek dosya
webhook-inspector — Webhook yakala, oku, localhost'a yeniden gönder
jwt-peek — JWT çözümleme ve doğrulama
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | 3 uç noktaya kadar, doğrulama + test | 150 USD | 3 gün |
| Standart | 10 uç nokta, kimlik doğrulama, veritabanı, Swagger | 450 USD | 7 gün |
| Premium | + Webhook alma/imza doğrulama, Docker, GitHub Actions ile CI | 900 USD | 12 gün |

---

### İlan 4 — Test yazma ve kod incelemesi

**Başlık:** `Mevcut Python/JavaScript projenize test yazma ve kod incelemesi`

```
Çalışan ama dokunmaya korktuğunuz bir kod tabanınız varsa: test yazıyorum
ve ne kırılmak üzere olduğunu raporluyorum.

Teslim:
• Testler — kolay olanı değil, kırılanı kapsayan. Saat dilimi sınırları,
  yuvarlama, boş girdi, eşzamanlı istek, zaman aşımı.
• Yazılı rapor: bulunan hatalar, ciddiyetine göre sıralı, her biri için
  "şu girdiyle şu olur" örneğiyle
• GitHub Actions kurulumu — testler her commit'te kendiliğinden koşsun

Güvenlik tarafına ayrıca bakıyorum: commit'e sızmış API anahtarı, SQL
enjeksiyonu, XSS, açık yönlendirme, imzasız webhook.

Düzeltmeleri de ben yapacaksam Premium paket.

Benzer açık kaynak işlerim: 21 projede 300'ün üzerinde test.
secretscan — Commit'e sızan anahtarları yakalayan pre-commit aracı
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek modül, kritik yollara test + kısa rapor | 90 USD | 2 gün |
| Standart | Proje geneli test + yazılı inceleme raporu + CI kurulumu | 300 USD | 5 gün |
| Premium | + Bulunan hataların düzeltilmesi ve refactor | 650 USD | 9 gün |

---

### İlan 5 — Vanilla JS bileşen ve sayfa hızı

**Başlık:** `Bağımlılıksız JavaScript ile web bileşeni ve sayfa hızı iyileştirme`

```
Framework kurmadan, tek dosyayla sayfanıza eklenen bileşenler yazıyorum
ve sayfa hızınızı ölçülebilir şekilde iyileştiriyorum.

Yaptıklarım:
• Özel bileşen (takvim, tablo, modal, galeri) — React ya da jQuery
  gerektirmeden, mevcut sayfaya script etiketiyle ekleniyor
• Görsel optimizasyonu: srcset üretimi, tembel yükleme, kendi yerini
  ayıran yer tutucu — Core Web Vitals'ta CLS'yi düşürür
• Erişilebilirlik: klavye ile kullanım, kontrast, ekran okuyucu etiketleri
• Koyu tema desteği

Ölçüm: işten önce ve sonra Lighthouse skorunu ekran görüntüsüyle
gönderiyorum. Fark yoksa ücret almıyorum.

Benzer açık kaynak işlerim:
lazy-img — Kendi yerini ayıran, srcset üreten, hatada yeniden deneyen
tembel görsel bileşeni
palette-lab — WCAG parlaklığına göre renk skalası
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek bileşen, duyarlı + koyu tema | 70 USD | 2 gün |
| Standart | Bileşen + erişilebilirlik + testler + dokümantasyon | 220 USD | 4 gün |
| Premium | Sayfa hızı denetimi + görsel optimizasyonu + önce/sonra raporu | 450 USD | 7 gün |

---

### İlan 6 — Türkçe karakter, para ve tarih hataları

**Başlık:** `Türkçe karakter, para birimi ve tarih/saat hatalarını düzeltiyorum`

```
Dar bir ilan, ama bu dört hatayı gerçekten çözüyorum — ve hemen her
projede var.

1. TÜRKÇE KARAKTER
'İstanbul'.toLowerCase() 8 değil 9 kod noktası üretir; istemediğiniz bir
birleşik nokta ekler. URL'lerde, aramada ve veritabanı karşılaştırmasında
ı/i/İ/I karışması buradan geliyor.

2. PARA VE YUVARLAMA
0.1 + 0.2 = 0.30000000000000004. Faturalar tam da bu yüzden bir kuruş
kayıyor. Parayı tam sayı kuruş olarak tutup öyle hesaplıyorum; KDV'yi
beyanname verilir gibi oran bazında grupluyorum.

3. TARİH VE SAAT DİLİMİ
Yaz saati geçişleri, UTC ile yerel saat karışması, arka plandaki sekmenin
saati şaşırması. Tik saymak yerine saati okuyan çözüm.

4. YENİDEN DENEME
Zaman aşımına uğramış bir POST isteği aslında başarılı olmuş olabilir —
körlemesine tekrar denemek kartı iki kez çeker. Doğrusu: üstel bekleme,
tam jitter, Retry-After başlığına uyma, POST'u varsayılan olarak tekrar
denememe.

Açık kaynak kanıtı:
slugify-tr, money-fmt, fetch-retry-lite, pomodoro-focus
github.com/antonidashaci
```

| Paket | İçerik | Fiyat | Süre |
|---|---|---|---|
| Temel | Tek hata sınıfı, tespit + düzeltme + test | 80 USD | 2 gün |
| Standart | Proje genelinde tarama, düzeltme, regresyon testleri | 250 USD | 4 gün |
| Premium | + Tekrarlamasını önleyen yardımcı modül ve CI kontrolü | 500 USD | 7 gün |

---

## 6. Profil tamamlama kontrol listesi

- [ ] Profil fotoğrafı — gerçek yüz, net, iyi ışık. Logo veya avatar değil.
- [ ] Kapak görseli — kod ekranı ya da düz renk; üstüne metin koyma.
- [ ] Profil başlığı (bölüm 1)
- [ ] Hakkımda (bölüm 2)
- [ ] Yetenek etiketleri, en az 10 (bölüm 3)
- [ ] Portfolyo — 8 giriş, her birinde ekran görüntüsü (bölüm 4)
- [ ] İlanlar — önce 3 tanesini yayınla, iki hafta sonra kalan 3'ü
- [ ] Her ilanda görsel: demo ekran görüntüsü ya da terminal çıktısı
- [ ] Kimlik doğrulama — rozet satış oranını belirgin şekilde artırıyor
- [ ] İlk hafta mesajlara 1 saat içinde dön; yanıt süresi sıralamayı etkiliyor

---

## 7. İlk 10 iş

İlk yorumlar her şeyi belirliyor. İlk 3-5 işi taban fiyatın altına al;
karşılığında detaylı yorum iste. Yorum sayısı 10'u geçince fiyatları
yukarıdaki seviyeye çek.

Teklif yazarken: ilanın kendi cümlelerinden birine değin (okuduğunu
gösterir), ardından o işe en yakın İKİ repoyu linkle. Beş link atmak
"okumadım" demektir.
