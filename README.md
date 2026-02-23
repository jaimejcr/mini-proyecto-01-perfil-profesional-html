# Mini proyecto 01 — Perfil profesional (solo HTML)

# Demo:
https://jaimejcr.github.io/mini-proyecto-01-perfil-profesional-html/

Perfil profesional en una sola página, creado exclusivamente con HTML para practicar y demostrar  estructura semántica, accesibilidad base y SEO técnico mínimo.

## Estado del proyecto

* Baseline actual: `index.html` 
* Objetivo: iterar sobre index.html hasta cumplir P0 (obligatorio), y después añadir P1/P2.

## Objetivo (qué demuestra este repo)

- Landmarks semánticos (`header`, `nav`, `main`, `footer`)
- Jerarquía correcta de headings (1 solo `h1`, `h2/h3` coherentes)
- Accesibilidad base (skip link, labels, alt, navegación clara por teclado)
- SEO técnico mínimo (title/description/robots/canonical/OG)
- Datos estructurados (JSON-LD)

## Alcance y restricciones

- Tecnología permitida: solo HTML (sin CSS, sin JavaScript)
- Entrega: `index.html` en la raíz del repositorio
- Assets opcionales: `/assets/` (imágenes, favicon)

## Estructura del repositorio

- `index.html`
- `README.md`
- `LICENSE`
- `assets/` (opcional)

## Checklist por niveles

### P0 (obligatorio)

Documento base

- `<!doctype html>`
- `<html lang="es">`
- `<meta charset="utf-8">`
- `<meta name="viewport" content="width=device-width, initial-scale=1">`
- Un solo `<main>` por página (`<main id="main-content">`)

Semántica y navegación

- `header` + `nav` + `main` + `footer`
- `nav` con `aria-label`
- Navegación interna por anclas (IDs en kebab-case)

Accesibilidad base

- Skip link funcional a `#main-content` como primer foco útil
- Orden de lectura lógico (DOM = lectura)
- Imágenes con `alt` significativo (o `alt=""` si son decorativas)
- Formularios: `label for` + `id` + `name` en inputs, `fieldset/legend` correctos
- Enlaces comprensibles (evitar “haz clic aquí”)

SEO técnico mínimo

- `title` único y descriptivo
- `meta name="description"` (texto real, sin relleno)
- `meta name="robots" content="index,follow"`
- `link rel="canonical"` (placeholder documentado, actualizar al publicar)
- Open Graph básico: `og:title`, `og:description`, `og:type`, `og:url`

Datos estructurados

- JSON-LD con `schema.org` tipo `Person` (name, jobTitle, url, sameAs)

Calidad

 HTML válido sin errores en W3C (0 errores)

### P1 (recomendado)

- Favicon real + `apple-touch-icon` (si aplica)
- `meta name="theme-color"`
- `figure/figcaption` para imágenes con contexto
- `abbr` para siglas (SEO, CWV) con `title`
- Sección “Notas técnicas” con `details/summary` (checklist + verificación)

### P2 (extras)

- `404.html` simple (si se publica con GitHub Pages)
- `humans.txt` o `robots.txt` (si se sirve como sitio)
- Versión bilingüe ES/EN como dos HTML distintos (opcional)

## Verificación (pruebas obligatorias)

1. W3C Validator

   - Validar `index.html` y corregir hasta 0 errores.

2. Lighthouse (Chrome DevTools)

   - Revisar SEO y Accesibilidad.
3. axe DevTools

   - Ejecutar auditoría y corregir issues relevantes (solo con HTML).
4. Navegación por teclado

   - Skip link primero y funcional.
   - Menú permite llegar a cada sección.
   - Si hay formulario, se completa con teclado.

## Publicación (GitHub Pages)

Se publicará con GitHub Pages cuando `index.html` cumpla P0.
Al publicar, actualizar:

- `canonical`
- `og:url`
  a la URL real del sitio.