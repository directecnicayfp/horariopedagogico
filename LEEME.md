# Horario Pedagógico · Educación Técnica Tucumán

Página web del horario pedagógico de las escuelas técnicas y agrotécnicas, publicada con GitHub Pages.

## Contenido

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página (diseño, logo y funcionamiento). |
| `datos/escuelas.json` | Lista de escuelas que se muestra en la portada. |
| `datos/<CUE>.json` | Horario completo de cada escuela (un archivo por escuela). |
| `.nojekyll` | Hace que GitHub Pages publique los cambios más rápido. |

## Editar un horario

1. Entrar a la escuela y tocar **Admin** (pide el PIN de la escuela).
2. La primera vez en cada computadora, completar **Conexión con GitHub** con un token (ver abajo).
3. Hacer clic en cualquier celda u horario y modificarlo. El cambio se guarda solo en el repositorio y queda visible para todos en aproximadamente un minuto.

Si no hay conexión, los cambios quedan guardados como borrador en ese navegador y se suben cuando se vuelve a entrar en Admin con la conexión configurada.

## Crear el token de GitHub

1. En GitHub: foto de perfil → **Settings** → **Developer settings** → **Personal access tokens** → **Fine-grained tokens** → **Generate new token**.
2. **Repository access** → **Only select repositories** → elegir solo este repositorio.
3. **Permissions** → **Contents** → **Read and write**.
4. Generarlo y pegarlo en la ventana **Conexión con GitHub** de la página.

El token queda guardado solo en el navegador donde se cargó. Quien tenga el token puede modificar el repositorio, así que no hay que compartirlo ni usarlo en computadoras públicas. El PIN de cada escuela solo bloquea el botón Admin; la protección real es el token.

## Agregar una escuela nueva

Subir su archivo `datos/<CUE>.json` (puede copiarse de otra escuela con **⬇ Copia** y editarse) y agregar una línea en `datos/escuelas.json` con `id`, `escuela`, `cue` y `cursos`.
