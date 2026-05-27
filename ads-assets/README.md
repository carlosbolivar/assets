# Tirami — Ad assets

Generated PNGs for **Google Ads**, **Meta** (Facebook / Instagram), **LinkedIn**, **TikTok**, and **X**.

Source files: `../../public/assets/branding/`

## Regenerar

```bash
cd "*DO NOT UPLOAD*/ads-assets"
npm install
npm run generate
```

## Estructura

| Carpeta | Uso |
|---------|-----|
| `google-ads/images/` | Performance Max / Display — tamaños Google |
| `google-ads/logos/` | Logos cuadrado 1:1 y apaisado 4:1 |
| `meta/images/` | Feed, Stories/Reels, link preview |
| `meta/logos/` | Perfil / wordmark |
| `linkedin/` | Sponsored content |
| `tiktok/` | Video cover vertical |
| `x-twitter/` | Promoted posts |
| `youtube/` | Thumbnails, Shorts, channel art |
| `universal/` | Exportaciones reutilizables + `sources/` |

## Google Ads (subir aquí)

### Imágenes

| Archivo | Tamaño | Ratio | Nota |
|---------|--------|-------|------|
| `landscape-1200x628.png` | 1200×628 | 1.91:1 | Desde `og-image.png` |
| `square-1200x1200.png` | 1200×1200 | 1:1 | Desde `tirami_square_4x.png` |
| `portrait-960x1200.png` | 960×1200 | 4:5 | **Contain** — logo no se corta |
| `tall-portrait-1080x1920.png` | 1080×1920 | 9:16 | **Contain** — logo no se corta |

Solo los **verticales** usan `contain` (el OG es apaisado). Horizontal y cuadrado igual que antes.

### Variantes con copy (EN / ES) — tipografía **DM Sans**

En `google-ads/images/variants/` (misma fuente que la landing). Requiere `fonts/DMSans-*.ttf` (incluidas).

| Archivo | Formato |
|---------|---------|
| `tall-portrait-1080x1920-en.png` / `-es.png` | 9:16 |
| `portrait-960x1200-en.png` / `-es.png` | 4:5 |
| `square-1200x1200-en.png` / `-es.png` | 1:1 |
| `landscape-1200x628-en.png` / `-es.png` | 1.91:1 |

### Logos

| Archivo | Tamaño | Notas |
|---------|--------|--------|
| `google-ads/logos/square-icon-1200x1200.png` | 1200×1200 | Icono `tirami.svg` sobre fondo marca |
| `google-ads/logos/square-wordmark-white-1200x1200.png` | 1200×1200 | Logo texto blanco (fondos oscuros) |
| `google-ads/logos/landscape-wordmark-white-1200x300.png` | 1200×300 | **Recomendado** logo apaisado 4:1 |
| `*-wordmark-dark-*` | — | Texto negro, fondo claro `#F4F3F5` |

## Meta (Facebook / Instagram)

| Archivo | Uso |
|---------|-----|
| `meta/images/feed-landscape-1200x628.png` | Feed / Advantage+ |
| `meta/images/feed-square-1080x1080.png` | Feed cuadrado |
| `meta/images/story-reels-1080x1920.png` | Stories, Reels |
| `meta/images/link-preview-1080x566.png` | Enlaces |
| `meta/logos/profile-icon-512x512.png` | Icono |
| `meta/logos/landscape-wordmark-white-1200x300.png` | Logo horizontal |

## Otras plataformas

- **LinkedIn:** `linkedin/images/landscape-1200x627.png`, `square-1080x1080.png`
- **TikTok:** `tiktok/images/video-cover-1080x1920.png`
- **X:** `x-twitter/images/landscape-800x418.png`, `square-800x800.png`

## YouTube

| Archivo | Uso |
|---------|-----|
| `youtube/images/video-thumbnail-1280x720.png` | Thumbnail de video (16:9) |
| `youtube/images/shorts-cover-1080x1920.png` | Cover para Shorts (9:16) |
| `youtube/images/channel-art-2560x1440.png` | Banner del canal |
| `youtube/logos/channel-icon-800x800.png` | Icono del canal / watermark |
| `youtube/logos/video-watermark-150x150.png` | Watermark para videos (fondo transparente) |
| `youtube/logos/channel-wordmark-white-2560x1440.png` | Wordmark blanco para fondos oscuros |
| `youtube/logos/channel-wordmark-dark-2560x1440.png` | Wordmark oscuro para fondos claros |

También se generan variantes con copy EN/ES en:
`youtube/images/variants/video-thumbnail-1280x720-*.png` y
`youtube/images/variants/shorts-cover-1080x1920-*.png`.

## Origen de cada creatividad

- **Imágenes marketing:** recorte de `og-image.png` (mismo arte que Open Graph).
- **Logos:** render desde SVGs en branding (`tirami.svg`, `tirami_logo_text_white.svg`, etc.).
- Fondo logo por defecto: `#211A1A` (neutral 900 de la landing).

## Notas

- Máx. 5120 KB por archivo (Google); estos PNG están optimizados.
- Si Google recorta, prioriza `landscape-1200x628` y `square-1200x1200`.
- Para variantes con copy en vivo, duplica en Figma usando `universal/sources/`.
