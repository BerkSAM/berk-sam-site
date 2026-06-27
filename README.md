# M. Berk SAM — Kişisel Web Sitesi

Tek dosyalık (vanilla + three.js), WebGL parçacık animasyonlu kişisel web sitesi.
"Kod & Özgürlük": yazılım/AI ile nomad/seyahat dünyasını tek bir bağlantı metaforunda birleştirir.

**Canlı dosya:** `index.html`

## Çalıştırma
Kurulum yok. Yerel sunucu yeterli (importmap için `file://` bazen çalışmaz):

```bash
python -m http.server 5173    # ya da: npx serve .
```
Sonra `http://localhost:5173` adresini aç.

## Öne çıkanlar
- **Scroll-driven morph:** Parçacık kütlesi bölümlere göre şekil değiştirir —
  🌐 dünya → 🕸️ canlı sistem ağı → 🍩 torus → 🛰️ yörünge/internet → 🌌 galaksi.
- **Anlatı:** Ne Yaptım · Ne Yapıyorum · Nomad · Gelecek · İletişim.
- **Sinematik nav:** Üst menüye tıklayınca kamera dalış + zoom geçişi yapar.
- **Kinetik tipografi:** Hero başlığı (Fraunces variable font) imlece tepki verir.
- **Özel imleç + manyetik linkler**, uçuş rotaları + ışık izleri, dünya rengi geçişi.
- **Erişilebilirlik & performans:** reduced-motion fallback, skip-link, focus state,
  frame-rate bağımsız `damp` animasyonlar, tab gizliyken render duraklatma.

## Teknik
three.js r160 (CDN importmap) · custom GLSL shader'lar · EffectComposer + UnrealBloom · GSAP yok, vanilla JS.

## Yapılacaklar
- Bölüm madde listelerini gerçek proje içeriğiyle doldurmak (bento grid'e dönüştürülebilir).
- İletişim linklerini (LinkedIn / GitHub / X / e-posta) güncellemek.
