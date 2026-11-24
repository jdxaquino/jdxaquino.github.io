---
id: CLD-JDXAQUINO-GITHUB-IO
version: "2.0"
title: "Guía de Claude Code del Sitio Personal"
doc_type: claude
project: jdxaquino-github-io
status: draft
phase: production
created: 2026-11-19
updated: 2026-11-24
evidence_cutoff: 2026-11-24
owner: Juan Jose D'Aquino Bautista
language: es
tags: [jdxaquino-github-io, sitio-personal, html-estatico, github-pages, claude]
related:
  - jdxaquino.github.io/README.md
  - jdxaquino.github.io/00-INDEX.md
  - CLAUDE.md
---

# CLAUDE.md — Sitio Personal (`jdxaquino.github.io`)

Contexto operativo de Claude Code en `jdxaquino.github.io/`, el sitio personal público de Juan Jose (`https://jdxaquino.github.io`). La portada es [`README.md`](README.md); las reglas del workspace `witsilin`, [`../CLAUDE.md`](../CLAUDE.md).


## 1. Alcance y Precedencia

- **Cubre:** la página publicada, su despliegue y su documentación.
- **Precedencia:** esta guía manda en lo particular del sitio; lo transversal (estilo, registros, contextos separados) vive en la guía del workspace.
- **Registros:** los pendientes del sitio van a [`../hub/deliverables/REVISIONES.md`](../hub/deliverables/REVISIONES.md) y las preguntas a [`../hub/deliverables/PREGUNTAS.md`](../hub/deliverables/PREGUNTAS.md).
- **Repositorio:** repo git con remoto `origin` en GitHub, público; lo que se commitea aquí se publica al hacer push.


## 2. Sitio y Despliegue

- **Página (`VERIFICADO`, `2026-11-24`):** un solo `index.html` sin dependencias externas (HTML, CSS y JS en línea), con botón ES/EN y tema claro/oscuro; el detalle de edición está en [`README.md`](README.md).
- **Despliegue:** GitHub Pages en modo *Deploy from a branch*, rama `main`, carpeta raíz; cada push a `main` publica.
- **Portafolio Astro Guardado:** la versión en Astro (componentes, mapa Leaflet, `deploy.yml`) vive solo en la rama local `astro-portfolio`, sin subir (`REV-017`); `.gitignore` excluye sus restos (`dist/`, `.astro/`, `node_modules/`).


## 3. Reglas para Trabajar Aquí

1. **Bilingüe Siempre:** todo texto existe como `<span data-l="es">` y `<span data-l="en">`; al editar se actualizan los dos.
2. **Confidencialidad (`BLOQUEANTE`):** el repo es público. Nunca incluyas nombres de tablas internas, credenciales, URLs de workspaces privados ni datos propietarios de empleadores o clientes; solo datos públicos o descripciones de alto nivel autorizadas.
3. **Nada de `hub/library/personal/`:** el material personal del hub (CV, documentos de RH, académicos) es sensible y no se copia al sitio sin instrucción de Juan Jose.
4. **Sin Commits ni Push sin Instrucción:** ningún asistente commitea ni hace push aquí sin instrucción explícita de Juan Jose.
5. **Documentación:** esta guía y el `00-INDEX.md` siguen el skill [`documentation-style`](../.claude/skills/documentation-style/SKILL.md) del workspace; el `README.md` es la cara pública del repo y conserva su formato.


## 4. Mantenimiento

- **Al Cambiar el Sitio o el Despliegue:** actualizar [Sitio y Despliegue](#2-sitio-y-despliegue).
- **Validación:** Juan Jose D'Aquino Bautista.
