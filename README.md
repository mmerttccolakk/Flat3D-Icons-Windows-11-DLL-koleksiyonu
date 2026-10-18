# Flat3D Icons — Windows 11 için kategorilere ayrılmış ikon DLL'leri

![ikon sayısı](https://img.shields.io/badge/ikon-3512-blue) ![platform](https://img.shields.io/badge/platform-Windows%2011%20x64-0067c0) ![format](https://img.shields.io/badge/format-icon%20resource%20DLL-green)

Windows 11'de kısayol, klasör ve dosya türü ikonlarını değiştirmek için hazırladığım, **3512 renkli ve 3B görünümlü ikon**. İkonlar **53 kategoriye ayrılmış DLL** içinde: bayraklar, sosyal medya logoları, araçlar, bankacılık, Linux logoları, günlük hayat nesneleri ve daha fazlası. Her DLL küçük olduğu için simge seçme penceresi hızlı açılıyor.

![Önizleme](docs/onizleme.jpg)

> English: 3512 colorful 3D-style icons split into 53 category-based resource-only DLLs (x64) for customizing shortcut, folder and file-type icons on Windows 11. See [INDEX.csv](INDEX.csv) for the DLL file and resource ID of every icon.

## İçindekiler

- [DLL listesi](#dll-listesi)
- [Kurulum ve kullanım](#kurulum-ve-kullanım)
- [Hangi DLL'de hangi ikon?](#hangi-dllde-hangi-ikon)
- [Kaynak koddan derleme](#kaynak-koddan-derleme)
- [Lisans ve kaynaklar](#lisans-ve-kaynaklar)
- [Önemli notlar](#önemli-notlar)

## DLL listesi

Hepsi [`dll/`](dll/) klasöründe. Her DLL'de ikon numaraları 101'den başlar.

| DLL | İkon sayısı | Boyut | İçerik |
|---|---:|---:|---|
| `windows11-modern.dll` | 119 | 4.2 MB | Windows 11 işlevlerinin modern karşılıkları (Bu Bilgisayar, Ayarlar, Görev Yöneticisi, Terminal, klasör türleri…) |
| `ubuntu-gnome-uygulamalar.dll` | 62 | 2.2 MB | Ubuntu / GNOME tarzı uygulama ve sistem ikonları |
| `navigasyon.dll` | 48 | 1.7 MB | Rota, GPS, yön okları, harita, trafik |
| `elektrik-su-dogalgaz.dll` | 53 | 1.9 MB | Elektrik, su, doğalgaz, sayaç, fatura |
| `emlak-konut.dll` | 56 | 2.0 MB | Dükkan, daire, arsa, villa, tapu, satılık/kiralık |
| `park-otopark.dll` | 61 | 2.1 MB | Park yeri, park no (01–30), kat/blok, engelli, ücretli |
| `denizcilik-su.dll` | 31 | 1.1 MB | Denizcilik, deniz, göl, su |
| `sigorta.dll` | 15 | 0.5 MB | Kasko, trafik, sağlık, konut sigortası |
| `okul-cv.dll` | 45 | 1.6 MB | Üniversite, lise, CV, sınavlar, diploma |
| `devlet-hizmetleri.dll` | 23 | 0.8 MB | Genel e-devlet / kamu hizmeti ikonları |
| `ios-ek.dll` | 30 | 1.1 MB | iOS ayar ve uygulama tarzı ek ikonlar |
| `google-yandex-servisleri.dll` | 47 | 1.7 MB | Google ve YouTube servisleri |
| `tr-ru-hizmet-markalari.dll` | 7 | 0.3 MB | Türkiye / Rusya servisleri |
| `sosyal-ve-servis-logolari.dll` | 87 | 3.2 MB | Sosyal medya, mesajlaşma, alışveriş, ödeme ve yayın servisleri |
| `teknoloji-oyun-markalari.dll` | 40 | 1.5 MB | Donanım, işlemci ve oyun platformu markaları |
| `arac-markalari.dll` | 47 | 1.8 MB | Otomobil ve motosiklet markaları |
| `kripto-coin.dll` | 31 | 1.2 MB | Kripto paralar, borsalar ve cüzdanlar |
| `linux-yazilim-ubuntu.dll` | 156 | 5.9 MB | Linux dağıtımları, masaüstü ortamları, geliştirici ve açık kaynak yazılım logoları |
| `harf-monogram-markalar.dll` | 82 | 2.8 MB | Resmi logosu açık lisanslı sette bulunmayan markalar için harf tabanlı genel ikonlar |
| `emoji-3d-ek-denizcilik-konut-enerji.dll` | 99 | 5.5 MB | 3B ek ikonlar (deniz canlıları, yapı, enerji, güvenlik) |
| `aktivite-spor.dll` | 82 | 4.9 MB | Spor ve aktiviteler (3B) |
| `apple.dll` | 6 | 0.2 MB | Apple ekosistemi logoları |
| `bayraklar.dll` | 245 | 11.9 MB | Ülke bayrakları (3B dalgalı) |
| `bilgisayar-cihaz.dll` | 38 | 1.9 MB | Bilgisayar ve elektronik cihazlar (3B) |
| `binalar-yerler.dll` | 24 | 1.5 MB | Binalar ve mekanlar (3B) |
| `dogal-gokyuzu.dll` | 87 | 5.1 MB | Doğa, gökyüzü, hava durumu (3B) |
| `finans-belgeler.dll` | 58 | 2.0 MB | Finans ve belge ikonları |
| `nesneler.dll` | 135 | 7.5 MB | Günlük nesneler (3B) |
| `para-belgeler.dll` | 65 | 3.1 MB | Para ve belge nesneleri (3B) |
| `semboller.dll` | 74 | 4.0 MB | Semboller ve işaretler (3B) |
| `teknoloji.dll` | 73 | 2.6 MB | Teknoloji ve geliştirici ikonları |
| `ulasim.dll` | 60 | 3.5 MB | Araç ve ulaşım (araba, tır, uçak, gemi, tren…) |
| `yazilim.dll` | 5 | 0.2 MB | Yazılım ve servis logoları |
| `arac-yakit-bakim.dll` | 51 | 1.8 MB | KM, litre, benzin/dizel, yağ, bakım, park, yük |
| `bankacilik-islemler.dll` | 30 | 1.0 MB | Banka, gişe, havale/EFT, işlem ve hesap ikonları |
| `bayraklar-yuvarlak.dll` | 259 | 13.5 MB | Ülke bayrakları (yuvarlak, parlak) |
| `bilgisayar-ag.dll` | 52 | 1.8 MB | Bilgisayar, ağ, dosya türleri, çevre birimleri |
| `harfler-rakamlar.dll` | 110 | 3.6 MB | A–Z, Türkçe harfler, Kiril harfleri, rakamlar, işaretler |
| `hayvan-bitki.dll` | 141 | 8.8 MB | Hayvanlar ve bitkiler (3B) |
| `insan-meslek-el.dll` | 111 | 7.2 MB | Meslekler ve el hareketleri (3B) |
| `ios-macos-tarzi.dll` | 80 | 2.7 MB | iPhone / iPad / Mac tarzı uygulama ve cihaz ikonları |
| `is-meslek.dll` | 16 | 0.6 MB | İş hayatı ve meslek ikonları |
| `kart-sim.dll` | 26 | 0.9 MB | Kredi kartı, SIM kart, eSIM |
| `kimlik-kart-belge.dll` | 24 | 0.9 MB | Kimlik, ehliyet, pasaport, belge ikonları (genel tasarım) |
| `muzik-dil.dll` | 45 | 1.6 MB | Müzik, şarkı, dil rozetleri (EN/RU/TR…) |
| `para-birimleri.dll` | 66 | 2.6 MB | TL, RUB, USD, EUR… para birimi, jeton ve banknot ikonları |
| `plakalar.dll` | 28 | 0.8 MB | Ülke plakaları (genel tasarım) |
| `universite-egitim.dll` | 14 | 0.5 MB | Eğitim ve okul ikonları |
| `yapay-zeka-guvenlik.dll` | 40 | 1.4 MB | Yapay zeka, şifre, anahtar, güvenlik, tehlike |
| `yemek-icecek.dll` | 127 | 7.5 MB | Yiyecek ve içecekler (3B) |
| `ev-mutfak-aletler.dll` | 21 | 0.7 MB | Ev, mutfak ve ev aletleri |
| `saglik-bakim.dll` | 11 | 0.4 MB | Sağlık ve kişisel bakım |
| `orijinal-small-flat-icons-dll.dll` | 169 | 10.6 MB | İlk DLL'den çıkarılan 169 orijinal düz ikon |

Her ikon 16, 32, 48, 64 ve 256 piksel boyutlarını içerir; arka plan şeffaftır.

## Kurulum ve kullanım

1. İstediğin DLL'leri (ya da hepsini) kalıcı bir klasöre koy, örneğin `C:\Icons\`.
2. İndirdikten sonra dosyaya sağ tıkla → **Özellikler** → engelleme varsa **Engellemeyi kaldır** kutusunu işaretle.

> DLL'i sildiğin ya da taşıdığın anda, onu kullanan tüm kısayol ve klasörlerin ikonları kaybolur. Bu yüzden kalıcı bir yere koy.

**Kısayol ikonunu değiştirmek**

1. Kısayola sağ tıkla → **Özellikler** → **Kısayol** sekmesi → **Simge Değiştir…**
2. Yola örneğin `C:\Icons\bayraklar.dll` yaz ve Enter'a bas.
3. Listeden ikonu seç, **Tamam**'a bas.

**Klasör ikonunu değiştirmek**

1. Klasöre sağ tıkla → **Özellikler** → **Özelleştir** sekmesi → **Simge Değiştir…**
2. Aynı şekilde DLL yolunu yaz ve ikonu seç.

**Dosya türü ikonunu değiştirmek**

Windows bunu doğrudan sunmuyor. [FileTypesMan](https://www.nirsoft.net/utils/file_types_manager.html) ya da [Winaero Tweaker](https://winaero.com/winaero-tweaker/) gibi araçlarla ilgili uzantıya bu DLL'lerden bir ikon atayabilirsin.

## Hangi DLL'de hangi ikon?

[`INDEX.csv`](INDEX.csv) dosyası her ikonun **DLL adını**, **kaynak numarasını**, kategorisini ve adını listeler:

```csv
dll,resource_id,kategori,ad
bayraklar.dll,101,bayraklar,flag-afghanistan
bayraklar.dll,102,bayraklar,flag-albania
...
```

Ad ve kategori İngilizce/Türkçe karışık kısa isimlerdir (örn. `park-no-07`, `logo-github`, `flag-turkey`).

## Kaynak koddan derleme

DLL'ler içinde kod olmayan, sadece ikon kaynaklarından oluşan DLL'lerdir. Kendin derlemek istersen:

1. İkonları `.ico` dosyaları olarak hazırla (küçük boyutlar BMP, 256 piksel PNG).
2. Her ikonu bir `.rc` dosyasına numarasıyla ekle:

```rc
101 ICON "ico/101.ico"
102 ICON "ico/102.ico"
```

3. Boş bir giriş noktası olan küçük bir C dosyası yaz (`stub.c`):

```c
int __stdcall DllMain(void *h, unsigned long r, void *p) { return 1; }
```

4. [Zig](https://ziglang.org/) ile çapraz derle (Windows gerekmez):

```bash
zig cc -target x86_64-windows-gnu -shared -nostdlib -Wl,--entry=DllMain -o bayraklar.dll stub.c bayraklar.rc
```

(Windows'ta MSVC `rc.exe` + `link /DLL /NOENTRY /MACHINE:X64 icons.res` ile de derlenebilir.)

## Lisans ve kaynaklar

İkonların büyük bölümü açık lisanslı setlerden üretildi veya bu setlerin stilinde kendim çizdim:

| Kaynak | Kullanım | Lisans |
|---|---|---|
| [Microsoft Fluent Emoji](https://github.com/microsoft/fluentui-emoji) | 3B nesne, bayrak, araç vb. ikonlar | MIT |
| [Simple Icons](https://github.com/simple-icons/simple-icons) | Marka logoları | CC0 |
| [Tabler Icons](https://github.com/tabler/tabler-icons) | Sistem, teknoloji, belge, navigasyon vb. glifler | MIT |
| [flag-icons](https://github.com/lipis/flag-icons) | Yuvarlak bayraklar | MIT |

Kimlik, ehliyet, pasaport, kredi kartı, plaka ve SIM kart ikonları genel tasarımlardır; resmi belge görselleri değildir. Bu projedeki kendi kodum ve çizimlerim için lisans: **MIT** (`LICENSE` dosyasına bakın). Üçüncü taraf ikonlar kendi lisanslarına tabidir.

## Önemli notlar

- **Marka logoları ilgili şirketlerin ticari markasıdır.** Bu proje bu şirketlerle bağlantılı değildir ve onlar tarafından onaylanmamıştır. Logoları kişisel masaüstü özelleştirmesi için kullanıyorum; ticari bir üründe kullanacaksan marka kurallarına bak.
- **Windows 11'in kendi ikonları kopyalanmadı.** `windows11-modern` kategorisi, Windows'taki işlevlerin (Bu Bilgisayar, Ayarlar, Görev Yöneticisi vb.) modern ve orijinal karşılıklarıdır; macOS/iPhone/Ubuntu tarzı ikonlar da aynı şekilde kendi çizimlerimdir.
- Resmi logosu açık lisanslı setlerde bulunmayan bazı markalar (Yandex, Trendyol, Sber, e-Devlet, Gosuslugi vb.) için resmi logo yerine harf tabanlı veya genel ikonlar kullandım (`harf-monogram-markalar`, `devlet-hizmetleri`).
- Sadece **64 bit** DLL üretildi.
- Pull request ve ikon önerilerine açığım.
