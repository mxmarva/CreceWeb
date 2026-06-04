# Manual de usuario — App móvil (CreceApp)

Documentación para socios, recepción, entrenadores y personal que usa **CreceApp**.

## URL en el servidor web

**`https://www.crecesportclub.com/manual_app/`**

El servidor abre **`index.html`** automáticamente en esa ruta.

## Editar contenido

1. Modifica **`source/body.html`**.
2. Regenera desde **Crece-Backend**:

```bash
python scripts/generate_user_manuals.py
```

## Publicación

Commit de `index.html`, `css/` y `source/body.html` en CreceWeb. Verifica `/manual_app/` tras el deploy.
