# Portafolio Docente

Sitio estático (HTML + CSS, sin dependencias de build) para publicar en GitHub Pages.

## Cómo subirlo al repositorio

1. Cloná tu repo (si no lo tenés local):
   ```
   git clone https://github.com/maristiaran/portafolio-docente.git
   ```
2. Copiá dentro de esa carpeta los archivos de este paquete: `index.html`, `assets/`, `materias/`.
3. Confirmá y subí los cambios:
   ```
   git add .
   git commit -m "Agregar portafolio docente y Unidad 2 de SO1"
   git push
   ```

## Cómo activar GitHub Pages

1. En GitHub, entrá a tu repositorio > **Settings** > **Pages**.
2. En "Build and deployment" > **Source**, elegí **Deploy from a branch**.
3. Seleccioná la rama `main` (o `master`) y la carpeta **/ (root)**.
4. Guardá. En 1-2 minutos tu sitio va a estar disponible en:
   `https://maristiaran.github.io/portafolio-docente/`

No hace falta `_config.yml` ni tema Jekyll: el sitio es HTML plano, ya con su propio estilo.

## Estructura

```
index.html                       → portada: recorrido B2 y materiales
assets/style.css                 → estilos compartidos
assets/insignia1-meme.png        → meme de la Insignia 1
entradas/01..04-*.html           → entradas del portafolio (una por módulo)
materias/so1/index.html          → Sistemas Operativos 1
materias/so1/unidad2.html        → apuntes de la Unidad 2 (CC BY-SA 4.0)
materias/so1/ruta-unidad2.html   → ruta de aprendizaje (Módulo 1)
```

## Agregar más materias o unidades

- Para una nueva unidad de SO1: creá `materias/so1/unidad3.html` (copiá la estructura de `unidad2.html`) y agregá una tarjeta en `materias/so1/index.html`.
- Para una materia nueva: creá `materias/<nombre>/index.html` y agregá una tarjeta en `index.html` (portada).
