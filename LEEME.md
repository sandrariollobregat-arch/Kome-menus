# Kome — cómo tener el icono en tu iPhone

Claude no puede publicar una app nativa en la App Store (eso requiere Xcode,
una cuenta de desarrollador de Apple y revisión de Apple). Pero esta carpeta
es una **app web instalable**: una vez publicada en una dirección propia,
podrás añadirla a tu pantalla de inicio con su icono, y se abrirá a
pantalla completa como una app normal, sin la barra de Safari.

## 1. Publica los archivos (elige una opción, las dos son gratis)

**Opción fácil — Netlify Drop** (sin cuenta ni instalar nada):
1. Ve a https://app.netlify.com/drop desde el ordenador.
2. Arrastra esta carpeta completa (`kome-standalone`) a la página.
3. Te dará una URL tipo `https://algo-al-azar.netlify.app`. Ábrela para comprobar que funciona.

**Opción alternativa — GitHub Pages:**
1. Crea un repositorio nuevo en GitHub y sube todos estos archivos.
2. En Settings → Pages, activa GitHub Pages sobre la rama principal.
3. Te dará una URL tipo `https://tuusuario.github.io/turepo`.

Importante: no sirve con abrir `index.html` haciendo doble clic en el
ordenador (protocolo `file://`) — necesita estar servida por una de estas
webs para funcionar correctamente.

## 2. Añádela a la pantalla de inicio del iPhone

1. Abre la URL publicada con **Safari** en el iPhone (tiene que ser Safari, no Chrome).
2. Toca el icono de compartir (el cuadrado con la flecha hacia arriba).
3. Baja y toca **"Añadir a pantalla de inicio"**.
4. Confirma el nombre ("Kome") y toca **Añadir**.

A partir de ahí tendrás el icono del onigiri en tu pantalla de inicio, y al
abrirla se abrirá a pantalla completa, como una app.

## Notas
- Todos los datos (rebost, menús, favoritos, histórico) se guardan solo en
  el propio iPhone mediante el almacenamiento del navegador. No se envían a
  ningún servidor ni a terceros.
- Si más adelante quieres cambiar recetas o colores, todo el código de la
  app está en `app.jsx`, en texto plano y comentado por secciones.
