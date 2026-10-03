# Instalar tu perfil de GitHub

Usuario: **CesarLopez-0124**

## 1. Agregar los GIFs

Descomprime el ZIP. Descarga dos GIFs de Dudu y guárdalos dentro de `CesarLopez-0124/assets/` como:

- `dudu-hello.gif`
- `dudu-coding.gif`

Las rutas ya están activas en el README. Hasta que agregues esos archivos, se verán como imágenes faltantes. Consulta `assets/LEEME-GIFS.txt`.

## 2. Crear el repositorio

En https://github.com/new crea un repositorio **público** llamado exactamente `CesarLopez-0124`. Si ya existe, usa ese repositorio y conserva cualquier archivo que quieras mantener antes de reemplazar el README.

El archivo `README.md` debe estar directamente en la raíz del repositorio, sin una carpeta extra llamada `CesarLopez-0124` dentro.

## 3. Subir los archivos

En GitHub, usa **Add file > Upload files** y sube el contenido de la carpeta descomprimida:

- `README.md`
- `assets/`, con el encabezado y tus dos GIFs.
- `.github/workflows/snake.yml`
- `INSTRUCCIONES.md` (opcional).

No subas el ZIP como un único archivo: GitHub no lo descomprime.

**Ojo con `.github`:** algunas interfaces ocultan las carpetas que comienzan con punto. Si no logras subirla, usa **Add file > Create new file** y escribe como nombre `.github/workflows/snake.yml`. Copia el contenido del archivo incluido y guarda el cambio en `main`.

## 4. Generar la serpiente

Abre la pestaña **Actions**, selecciona **Generate contribution snake**, pulsa **Run workflow** y confirma la ejecución en tu rama principal. El workflow también se ejecuta al subir su archivo a `main` o `master`, y queda programado diariamente.

Cuando termine con una marca verde, existirá una rama `output` con los SVG. La imagen del perfil aparecerá al actualizar la página; puede tardar unos minutos por la caché. No necesitas activar GitHub Pages ni crear un token personal: usa el token automático de Actions.

Si aparece un error de permisos al publicar, revisa **Settings > Actions > General > Workflow permissions**. El workflow solicita `contents: write`; una restricción del repositorio o de la organización puede bloquearlo. Si la opción está disponible, habilita **Read and write permissions** y vuelve a ejecutar. Si no ves Actions, revisa que estén habilitadas para ese repositorio.

## 5. Ver tu perfil

Abre https://github.com/CesarLopez-0124.

El README incluye un encabezado local, presentación, tecnologías, estadísticas, lenguajes más usados, Snake y dos espacios para Dudu. GitHub controla el fondo general del perfil; el encabezado y las tarjetas tienen un estilo oscuro y azul.

Las tarjetas de estadísticas y los iconos usan servicios externos. Las estadísticas pueden fallar temporalmente por límites del servicio; los lenguajes muestran uso en repositorios públicos y no miden tu nivel de conocimiento. El workflow se verificó por estructura, pero su ejecución real se realiza después de subirlo a GitHub. Las tareas programadas de repositorios públicos pueden desactivarse tras 60 días sin actividad; puedes habilitarlas otra vez desde Actions.

## Fuentes

- README de perfil: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- Snake: https://github.com/Platane/snk
- Publicación de SVG: https://github.com/peaceiris/actions-gh-pages
- Tarjetas de estadísticas: https://github.com/anuraghazra/github-readme-stats
- Iconos: https://github.com/tandpfun/skill-icons
