# Concentric Lab — Sitio Web Oficial

Sitio web de **Concentric Lab** — laboratorio digital de UX/UI, IA y automatización desde Bogotá, Colombia.

## ¿Para qué sirve este README?

El README es el primer documento que ve cualquier persona que abra el repositorio en GitHub. Sirve para:
- Explicar qué es el proyecto y cómo está estructurado
- Documentar cómo instalar, correr o deployar el sitio
- Dejar pendientes y notas de configuración para el equipo (o para ti mismo en el futuro)

---

## Stack

- **HTML / CSS / JS puro** — sin frameworks, cero dependencias de build
- **Fuentes:** Inter (Google Fonts) + Cal Sans (jsDelivr/fontsource)
- **Formulario:** Formspree (`xreoreqr`) — ya configurado
- **Deploy:** GitHub Pages o Netlify (drag & drop o CI automático)

---

## Estructura del proyecto

```
concentriclab/
├── index.html              ← sitio completo (HTML + CSS + JS inline)
├── assets/
│   ├── images/             ← todos los assets de imagen
│   │   ├── logo.png
│   │   ├── favicon.png
│   │   ├── og-image.png
│   │   ├── hero-1.webp
│   │   ├── hero-2.webp
│   │   ├── hero-3.webp
│   │   ├── enfoque-label.png
│   │   ├── producto-1.webp
│   │   ├── principio-1.webp
│   │   ├── principio-2.webp
│   │   ├── principio-3.webp
│   │   ├── yt-thumbnail.webp
│   │   ├── contact-bg.webp
│   │   ├── footer-bg.webp
│   │   └── gumroad-icon.svg
│   └── videos/
│       └── stats-bg.mp4    ← video de fondo sección manifiesto
└── README.md
```

---

## Cómo deployar

### Opción A — GitHub Pages (recomendado para control de versiones)
1. Sube todos los archivos a un repositorio en GitHub
2. Ve a **Settings → Pages → Source → Deploy from branch → `main` → `/root`**
3. GitHub genera la URL automáticamente (ej. `tu-usuario.github.io/concentriclab`)

### Opción B — Netlify (más rápido, drag & drop)
1. Ve a [netlify.com/drop](https://netlify.com/drop)
2. Arrastra la carpeta completa del proyecto
3. URL disponible en segundos

### Dominio propio
Cuando tengas dominio (`concentriclab.com`):
1. En Netlify/GitHub Pages: configura el dominio custom en Settings
2. Busca `TODO` en `index.html` y actualiza la URL canónica
3. Usa **Cloudflare Registrar** para el registro más barato + Cloudflare Pages para hosting gratuito

---

## Configuración pendiente

- [x] Formspree configurado — ID: `xreoreqr`
- [ ] Actualizar URL canónica en `<head>` cuando tengas dominio propio
- [ ] Crear productos "Blueprint Make/n8n" y "UI Kit Figma" cuando estén listos
- [ ] Agregar link real de Notion Store al botón "Descarga en Notion"
- [ ] Subir más videos al canal de YouTube para activar sección de contenido

---

## Funcionalidades del sitio

| Feature | Descripción |
|---|---|
| **Modo oscuro / claro** | Guardado en `localStorage`, respeta `prefers-color-scheme` del sistema |
| **Bilingüe ES / EN** | Sistema i18n propio, sin librerías externas |
| **Animación letra por letra** | El párrafo de Enfoque anima cada carácter individualmente al hacer scroll |
| **Slider de principios** | Autoavance cada 6s, swipe táctil, dots y flechas |
| **Cursor personalizado** | Solo en desktop con mouse (pointer:fine) |
| **Contador animado** | Los números del manifiesto se animan al entrar en viewport |
| **Progress bar** | Barra de progreso de scroll en la parte superior |
| **Newsletter** | Integrado con Formspree, envío AJAX sin recarga |

---

## Paleta de colores

| Variable | Valor | Uso |
|---|---|---|
| `--blue` | `rgb(80,90,245)` | Color principal de marca |
| `--salmon` | `rgb(244,120,85)` | Coral de marca, acentos cálidos |
| `--pink` | `rgb(255,130,225)` | Acentos secundarios |
| `--blue-lt` | `rgb(130,138,255)` | Versión clara del azul (secciones dark) |

---

## Créditos

Diseño, desarrollo y contenido: **Concentric Lab**  
Bogotá, Colombia · 2026  
[concentriclab.com](https://concentriclab.com) · [@concentriclab](https://instagram.com/concentriclab)
