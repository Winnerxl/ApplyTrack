# ApplyTrack

Basit, sunucusuz (serverless) **iş başvuru takip** aracı. Başvurularınızı tablo, **zaman grafiği** ve **Avrupa haritası** ile görselleştirir. **Wishlist** ile düşündüğünüz pozisyonları kaydedip tek tıkla başvurulara taşıyın.

## ✨ Özellikler
- %100 istemci tarafı: veri **localStorage**’da kalır
- CSV / JSON dışa & içe aktarma
- Filtreleme, sıralama, klavye kısayolları (`/`, `Ctrl+Enter`)
- ECharts ile **Avrupa ısı haritası** ve **zaman serisi grafiği**
- **Wishlist (Başvurulmak İstenen İşler) → Başvurulara Taşı**  
- Açık/Koyu tema


> **⚠️ Uyarı (localStorage & file://)**  
> ApplyTrack verileri tarayıcınızın **localStorage** alanında, **origin** (köken) bazlı tutar.  
> Dosyayı `file://` ile farklı klasör/isimden açarsanız tarayıcı bunu farklı bir origin sayar ve veriler ayrı görünebilir.  
> Bu nedenle sayfanın üstünde bir **banner uyarısı** gösteriyoruz (JSON yedekle / Kapat / Bir daha gösterme).  
> **Öneri:** Projeyi **GitHub Pages**’ten çalıştırın veya yerelde **localhost** üzerinden açın.

## 📦 Kullanım
Kurulum gerekmez. Bu depoyu indirin/klonlayın ve `index.html` dosyasını bir tarayıcıda açın.

- **Veri Saklama:** Tarayıcınızın `localStorage` alanı (cihaza özeldir).
- **Dışa Aktar:** `.json` veya `.csv`
- **İçe Aktar:** `.json` yükleyin.

### Yerelde Çalıştırma (önerilir)
`file://` kaynaklı origin farklarını yaşamamak için küçük bir statik sunucu kullanın:

**Python**
```bash
cd ApplyTrack
python3 -m http.server 5173
# http://localhost:5173/
```

## 🔒 Gizlilik
Verileriniz yalnızca tarayıcınızda tutulur; sunucuya gönderilmez.

## 🗺 Teknolojiler
- HTML/CSS/JS
- [Apache ECharts 5](https://echarts.apache.org/)
- Public GeoJSON kaynakları

## 📄 Lisans
MIT — bkz. `LICENSE`
