# Manual de usuario — Panel web

Documentación para el personal del club (panel **manage.crecesportclub.com** y kiosco **/acceso**).

## Editar contenido

1. Modifica **`body.html`** en esta carpeta (secciones con anclas `#intro`, `#caja`, etc.).
2. Regenera el manual completo desde **Crece-Backend**:

```bash
python scripts/generate_user_manuals.py
```

Eso actualiza **`index.html`** y copia estilos a `manual_app` si aplica.

## Cómo leerlo

1. Abre **`index.html`** en el navegador (misma carpeta que `css/manual.css`).
2. Usa el menú lateral para saltar de sección.
3. Usa el buscador del menú para filtrar temas.
4. En celular, **☰ Menú** abre la navegación.

## Publicación

Este repo (CreceWeb) suele publicarse en GitHub Pages u hosting del sitio del club. Haz commit de `body.html` e `index.html` tras regenerar.
