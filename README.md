# Concéntrico Lab — Web Principal

> Laboratorio digital de diseño, branding, IA y automatización · Bogotá para LATAM  
> https://concentricolab.vercel.app

---

## Stack

| Capa | Herramienta |
|------|------------|
| Hosting | Vercel (deploy automático desde GitHub) |
| Frontend | HTML + CSS + JS vanilla (un solo archivo `index.html`) |
| Fuentes | Cal Sans (display) · Inter (body) · vía CDN |
| Newsletter | Formspree — Form ID: `xreoreqr` |
| Animaciones | CSS keyframes + Intersection Observer |
| Dark mode | Toggle manual + `prefers-color-scheme` |
| i18n | ES / EN — objeto JS de traducciones en el mismo HTML |

---

## Estructura del repositorio

```
/
├── index.html          ← Sitio completo (todo en un archivo)
├── sitemap.xml         ← Sitemap para Google Search Console
├── assets/
│   ├── images/
│   │   └── og-image.png   ← Imagen para redes sociales (og:image)
│   ├── videos/
│   │   └── stats-bg.mp4   ← Video de fondo en sección manifiesto
│   └── fonts/             ← Cal Sans local (si aplica)
└── README.md
```

---

## Deploy

El deploy es automático: cualquier push a `main` activa un nuevo build en Vercel.

Para desplegar manualmente:
```bash
# Si tienes Vercel CLI instalado
vercel --prod
```

---

## SEO implementado (Abril 2026)

Todo el SEO vive dentro del `<head>` de `index.html`. No requiere configuración externa en Vercel.

**Activo automáticamente al hacer deploy:**
- `<title>` y `<meta description>` optimizados
- Open Graph completo (og:title, og:description, og:image con URL absoluta)
- Twitter Card
- `robots: index, follow`
- `author`, `keywords`, `theme-color`
- `hreflang` ES / EN / x-default
- Link a `sitemap.xml`
- Schema.org — Organization + WebSite + Productos (JSON-LD)

**Requiere acción manual de Camilo:**
1. Ir a [search.google.com/search-console](https://search.google.com/search-console)
2. Añadir propiedad: `concentricolab.vercel.app`
3. Verificar con el meta tag → pegarlo en el comentario del HTML donde dice `PEGA_TU_CÓDIGO_AQUÍ`
4. Enviar sitemap: ir a Sitemaps → escribir `/sitemap.xml` → Enviar

---

## Dark mode

Los fondos oscuros usan **`#00031F`** como base (no negro puro), preservando los efectos de glow y glass.

| Variable CSS | Valor dark |
|-------------|-----------|
| `--bg` | `#00031F` |
| `--bg-alt` | `#020425` |
| `--bg-dark-section` | `#010316` |
| `--dark` | `#00031F` |
| `--dark-glass` | `rgba(0, 3, 31, 0.85)` |

---

## Newsletter

El formulario usa Formspree con Form ID `xreoreqr`.  
Endpoint: `https://formspree.io/f/xreoreqr`  
Estado: ✅ Activo y funcional (bug de validación corregido en Abril 2026)

---

## i18n

El sitio tiene traducciones ES/EN completas implementadas como un objeto JS en el propio `index.html`. El idioma se alterna con el botón ES/EN en la barra de navegación.

---

## Mantenimiento

- **Añadir producto nuevo:** buscar `<!-- PRODUCTOS -->` en `index.html` y duplicar un bloque `.product-card`
- **Cambiar texto del hero:** buscar `hero_sub` en el objeto de traducciones (ES y EN)
- **Actualizar stack:** buscar `<!-- STACK -->` en `index.html`
- **Cambiar colores:** modificar las variables CSS en `:root` y en `.dark` al inicio del `<style>`

---

*Concéntrico Lab · Bogotá · 2025–2026*
