1 Qué es el repo

Mini proyecto 01 — Perfil profesional (solo HTML)

Baseline actual: práctica del curso (HTML puro) sobre la que se iterará.

2 Objetivo

Semántica + accesibilidad base + SEO técnico mínimo + JSON-LD.

3 Alcance

Solo HTML, sin CSS/JS por ahora.

Assets opcionales en /assets/.

4 Checklist por niveles

P0

doctype, lang, charset, viewport, un solo main

landmarks + nav con aria-label

skip link funcional

headings correctos (1 H1)

metadatos SEO: title/description/robots/canonical/OG

formulario accesible (label/for, name, fieldset/legend)

JSON-LD Person

W3C 0 errores

P1

favicon + theme-color

figure/figcaption, abbr, details/summary “Notas técnicas”

hreflang si bilingüe

P2

404.html, humans.txt/robots.txt, versión ES/EN

5 Verificación

W3C validator (0 errores)

Lighthouse/axe (sin fallos críticos)

navegación por teclado (skip link, foco lógico)

6 Publicación

GitHub Pages + actualizar canonical/og:url a la URL real.

# Mini proyecto 01 — Perfil profesional (solo HTML)

Perfil profesional en una sola página, creado exclusivamente con HTML para practicar estructura semántica, accesibilidad base y SEO técnico, con un estándar verificable tipo entrevista.

## Objetivo

Demostrar dominio real de HTML aplicando:

- Landmarks semánticos (header/nav/main/footer)
- Jerarquía correcta de headings
- Accesibilidad base (skip link, labels, alt, navegación clara)
- Metadatos SEO mínimos (title/description/canonical/OG)
- Datos estructurados (JSON-LD)

## Alcance y restricciones

- Permitido: solo HTML
- Entrega: `index.html` en la raíz del repositorio y assets opcionales (img/favicon)

## Estructura del repositorio

- `index.html`
- `README.md`
- `.gitignore`
- `assets/` (opcional)

## Checklist de requisitos (P0)

-   `<!doctype html>`, `lang="es"`, `meta charset`, `meta viewport`
-   Skip link funcional hacia `#main-content`
-   Landmarks: `header`, `nav`, `main`, `footer`
-   1 solo `h1` y jerarquía sin saltos (h2/h3 correctos)
-   Secciones mínimas: Hero, Experiencia, Proyectos, Habilidades, Formación, Contacto
-   Navegación interna por anclas 
-   Enlaces externos correctos 
-   Metadatos SEO: `title`, `meta description`, `robots`, `canonical`, OG básico
-   Datos estructurados: JSON-LD `Person` válido
-   HTML válido sin errores (W3C)

## Verificación (pruebas)

1. Validación HTML (W3C)
    - Validar index.html y corregir hasta 0 errores.
2. Lighthouse (Chrome DevTools)
    - Revisar secciones de SEO y accesibilidad.
3. axe DevTools (extensión)
    - Ejecutar auditoría y corregir errores relevantes.
4. Navegación por teclado
    - El skip link debe ser el primer elemento útil.
    - El menú debe permitir llegar a cada sección.
    - Si hay formulario, se debe completar solo con teclado.

## Publicación (GitHub Pages)

Publicaré la página con GitHub Pages cuando el index.html tenga la estructura P0 completa
