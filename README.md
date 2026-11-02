# LojiXcel – Lojistik için Excel AI

Lojistik ve tedarik zinciri ekipleri için Excel analiz aracı: tanıtım sitesi (Türkçe + İngilizce) ve tarayıcıda çalışan sevkiyat analizi uygulaması.

| Dosya | İçerik |
|---|---|
| `index.html` | Türkçe tanıtım sayfası |
| `en.html` | İngilizce tanıtım sayfası (English landing page) |
| `app.html` | Uygulama: Excel/CSV yükle → OTD/OTIF, taşıyıcı ve rota analizi, veri kalitesi raporu, Türkçe/İngilizce Excel formülleri, Excel’e aktarma |

Derleme adımı yoktur; her sayfa tek bir HTML dosyasıdır. Uygulama dosyaları hiçbir sunucuya göndermez, tüm hesaplama tarayıcıda yapılır.

## GitHub Pages ile yayınlama

1. GitHub’da yeni bir depo oluşturun ve bu klasördeki dosyaları (gizli `.nojekyll` dahil) depo köküne yükleyin.
2. **Settings → Pages → Build and deployment** bölümünde *Source: Deploy from a branch*, *Branch: main* ve */ (root)* seçip kaydedin.
3. Birkaç dakika içinde site `https://KULLANICI-ADI.github.io/DEPO-ADI/` adresinde yayında olur.

Yerelde denemek için `index.html` dosyasını tarayıcıda açmanız yeterlidir.

## Dış bağımlılıklar

- Google Fonts (Manrope, JetBrains Mono)
- SheetJS 0.18.5 (`cdnjs.cloudflare.com`): uygulamada .xlsx okuma/yazma için. İnternet yoksa yalnızca CSV dosyaları açılabilir.

## Yayına almadan önce değiştirin

- Örnek istatistikler (%70, 2 dk) ve temsilî kullanım senaryoları
- `href="#"` yer tutucu bağlantıları (giriş, ödeme, yasal sayfalar)
- `lojixcel.app` alan adı (canonical, hreflang ve Open Graph etiketleri)
- Fiyatlar ve plan limitleri
