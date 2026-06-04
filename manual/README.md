# Manual de usuario — Panel web

Documentación para el personal del club (panel **manage.crecesportclub.com** y kiosco **/acceso**).

## URL en el servidor web

En producción el personal abre solo:

**`https://www.crecesportclub.com/manual/`**

(o la ruta equivalente en tu dominio). El servidor debe servir **`index.html`** por defecto en esa carpeta (incluido `.htaccess` con `DirectoryIndex index.html`).

No enlaces ni compartas `source/body.html`; es solo la plantilla editable.

## Editar contenido

1. Modifica **`source/body.html`** (secciones con anclas `#intro`, `#caja`, etc.).
2. Regenera desde **Crece-Backend**:

```bash
python scripts/generate_user_manuals.py
```

Eso reconstruye **`index.html`** y sincroniza estilos con `manual_app`.

## Publicación

Haz commit de `index.html`, `css/` y `source/body.html` en **CreceWeb** y despliega el sitio. Tras el deploy, verifica que `/manual/` abre el manual completo con menú lateral.
