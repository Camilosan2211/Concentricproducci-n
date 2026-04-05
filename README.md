# Concentric Lab — Sitio Web

Sitio web oficial de **Concentric Lab** — laboratorio digital de UX/UI, IA y automatización desde Bogotá.

## Stack
- HTML/CSS/JS puro — sin frameworks
- Deploy en Netlify (drag & drop)
- Fuentes: Inter (Google Fonts) + Cal Sans (jsDelivr)

## Estructura
```
concentriclab/
├── index.html          ← sitio completo
├── assets/
│   ├── images/         ← descarga las imágenes de Framer CDN (ver lista abajo)
│   └── video/          ← descarga el video de fondo
└── README.md
```

## Imágenes pendientes de descargar
Descarga cada URL y guárdala con el nombre indicado en `assets/images/` o `assets/video/`:

| Archivo local | URL original |
|---|---|
| `assets/images/logo.png` | https://framerusercontent.com/images/hd58yXIN4R47jxZgWD19awres.png |
| `assets/images/favicon.png` | https://framerusercontent.com/images/i8vX66J3OcrRANITImxFn4WVoY.png |
| `assets/images/og-image.png` | https://framerusercontent.com/assets/NFKKkgn3P1xC3ZE4e3yv4VIeoM.png |
| `assets/images/hero-1.jpeg` | https://framerusercontent.com/images/rf2SDv1XBDB2J8J0Jc5rCqcm2U.jpeg |
| `assets/images/hero-2.jpeg` | https://framerusercontent.com/images/9uAvGuD7oMUyJdcTr62h13V7mjU.jpeg |
| `assets/images/hero-3.jpeg` | https://framerusercontent.com/images/4MKLmJBsDVZK97JDWqkAa17N3RU.jpeg |
| `assets/images/enfoque-label.png` | https://framerusercontent.com/images/UmIUDVWhypROFuonPgr1nDSTSjg.png |
| `assets/images/producto-1.png` | https://framerusercontent.com/images/BYbTfLPwKrQ8KDoRNlrCPLZwoj0.png |
| `assets/images/principio-1.jpeg` | https://framerusercontent.com/images/vSZyVOnLBagag5SXRINgQXDT1j0.jpeg |
| `assets/images/principio-2.jpeg` | https://framerusercontent.com/images/S5WQsuzNpNz4MTC6JhZVzDj4Vic.jpeg |
| `assets/images/principio-3.jpeg` | https://framerusercontent.com/images/8oe75LVG7p5S6V1RwBrzSHrAR0.jpeg |
| `assets/images/yt-thumbnail.png` | https://framerusercontent.com/images/YcYECqqfP3DEf1qBy7Ldk27rqbU.png |
| `assets/images/contact-bg.png` | https://framerusercontent.com/images/1sREGvYWbdhqXmijCOMUIsD7A.png |
| `assets/images/footer-bg.jpeg` | https://framerusercontent.com/images/eHn2ObLmY2s5f30XS3PFk7Pnv4.jpeg |
| `assets/images/gumroad-icon.svg` | https://framerusercontent.com/images/9oFUtuMBLGiKbIQAsGJZYO8sB4.svg |
| `assets/video/stats-bg.mp4` | https://framerusercontent.com/assets/3CTYWqZN338ZP9MTYUs5qYCvY.mp4 |

## Deploy en Netlify
1. Ve a [netlify.com/drop](https://netlify.com/drop)
2. Arrastra la carpeta completa del proyecto
3. ¡Listo! URL disponible en segundos

## Pendientes antes de producción final
- [ ] Descargar todas las imágenes listadas arriba
- [ ] Crear cuenta en [Formspree.io](https://formspree.io) y reemplazar `FORMSPREE_ID_AQUI` en index.html
- [ ] Actualizar canonical URL cuando tengas dominio propio (busca `TODO` en index.html)
