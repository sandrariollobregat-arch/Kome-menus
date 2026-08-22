# Arreglo: pantalla en blanco al abrir el icono

Ahora todo el código vive en un único `index.html` (ya no depende de un
segundo archivo `app.jsx`), así que hay mucho menos margen para que algo
se pierda al subirlo.

## Qué hacer en tu repositorio de GitHub

1. Entra en tu repo (`Kome-menus`) desde github.com en Safari.
2. Borra los archivos antiguos:
   - Toca `index.html` → icono de papelera (🗑) → confirma el borrado ("Commit changes").
   - Haz lo mismo con `app.jsx` si existe en el listado.
3. Sube los archivos nuevos de esta carpeta (`Add file` → `Upload files`,
   selecciona TODOS los archivos de esta carpeta) → `Commit changes`.
4. Espera 1-2 minutos a que GitHub Pages reconstruya el sitio.

## Después de subir: limpia la caché antes de probar

Esto es importante — Safari e iOS cachean agresivamente:

1. En el iPhone, borra el icono actual de la pantalla de inicio (mantén
   pulsado → Eliminar app).
2. Ve a Ajustes → Safari → Avanzado → Datos de sitios web. Busca
   "github.io", tócalo y elimínalo (esto borra la copia guardada de la
   página antigua).
3. Abre Safari, visita de nuevo tu URL
   (`https://sandrariollobregat-arch.github.io/Kome-menus/`) y comprueba
   que se ve bien la app (con colores y el menú).
4. Solo si se ve bien ahí, vuelve a hacer "Compartir" → "Añadir a
   pantalla de inicio".

Si al abrir la URL en Safari (paso 3) ves solo el texto "Cargando Kome…"
sin que desaparezca, el problema es que algún script externo (React,
Babel o las fuentes) no se está cargando — dímelo y seguimos desde ahí.
