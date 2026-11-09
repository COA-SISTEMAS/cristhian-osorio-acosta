# Cristhian Osorio Acosta — Exposición Artística

Sitio web personal para presentar la obra artística de Cristhian Osorio Acosta.

## Contenido

- `index.html`: página principal de la exposición.
- Catálogo de 16 obras con técnica, año y descripción.
- Galería visual e índice alternativo.
- Filtros por periodo.
- Visor ampliado con navegación por teclado y gestos táctiles.
- Presentación del artista y datos de contacto.
- Diseño adaptable a computadoras y dispositivos móviles.

## Recursos gráficos

- Los originales se conservan en la raíz del repositorio.
- `thumbs/`: miniaturas WebP para la galería.
- `optimized/`: versiones WebP de mayor resolución para el visor.

El flujo `optimize-images.yml` genera las dos variantes cuando se agregan o modifican originales PNG/JPG/JPEG. Los cambios en `index.html` ya no disparan una regeneración innecesaria de todas las imágenes.

## Automatizaciones

- `actualizar-contacto.yml`: valida que los enlaces de contacto, secciones y las 16 fichas del catálogo estén presentes. No modifica ni reemplaza el HTML.
- `optimize-images.yml`: genera imágenes WebP y publica únicamente los recursos derivados.

Ambos flujos declaran permisos explícitos y usan grupos de concurrencia para reducir ejecuciones simultáneas.

## Publicación

Sitio preparado para GitHub Pages desde la rama `main`.

## Desarrollo y revisión

Los cambios de mantenimiento deben prepararse en ramas independientes y revisarse mediante Pull Request antes de integrarse en `main`.
