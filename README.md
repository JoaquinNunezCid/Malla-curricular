# Malla interactiva de Ingeniería Mecatrónica — UNLZ

Sitio estático para que cada estudiante registre su avance de manera local y calcule el porcentaje de carrera ponderado por horas de las materias aprobadas.

## Características

- Malla de 49 materias con cargas horarias y correlativas transcritas a partir de una versión de referencia del plan.
- Porcentaje de avance calculado como horas aprobadas / 3.424 horas registradas.
- Filtros por materias aprobadas, disponibles y con correlativas pendientes.
- Guarda el progreso en el navegador, sin cuentas ni servidor de datos.
- Exportación e importación de respaldo JSON.
- Diseño adaptable a móviles y escritorio.
- No necesita compilación ni dependencias externas.

## Publicar en GitHub Pages

1. Iniciá sesión en GitHub y creá un repositorio nuevo, por ejemplo `malla-mecatronica-unlz`. Para que sea público, elegí **Public**.
2. En el repositorio, seleccioná **Add file → Upload files** y subí `index.html` desde esta carpeta. También podés subir este `README.md`.
3. Entrá a **Settings → Pages**.
4. En **Build and deployment**, elegí **Deploy from a branch**.
5. En **Branch**, seleccioná `main` y carpeta `/(root)`. Presioná **Save**.
6. Esperá a que termine el despliegue. En esa misma sección aparecerá la dirección pública, normalmente `https://TU-USUARIO.github.io/malla-mecatronica-unlz/`.
7. Abrí el enlace y probá marcar una materia, recargar la página y exportar un respaldo.

No hace falta usar Git, instalar programas ni ejecutar un proceso de build.

## Importante sobre el progreso

El progreso se almacena en `localStorage` del navegador y dispositivo de cada persona. No se comparte entre usuarios ni se sincroniza entre equipos. Cada estudiante debe usar **Exportar respaldo** para guardar su progreso en un archivo JSON y **Importar respaldo** para recuperarlo en otro dispositivo o navegador.

## Nota sobre la exactitud de la malla

La aplicación no es oficial ni está afiliada a la UNLZ. Los nombres de las materias, las 3.424 horas y las correlativas fueron transcritos de una versión de referencia disponible al desarrollar la herramienta. Antes de usar el porcentaje como dato académico oficial, contrastar la información con el plan de estudios vigente de la Facultad. El progreso es una estimación ponderada por horas, no necesariamente el porcentaje que informa SIU.

## Actualizar la aplicación

Editá `index.html` y subí el archivo actualizado al repositorio usando **Add file → Upload files**, o reemplazalo mediante un commit. GitHub Pages volverá a publicar el sitio.
