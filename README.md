# Huerta de Lola

Juego de granja para Android (uso personal). Plantás, regás, cosechás, cuidás animales y atendés clientes en el puesto.

## Cómo obtener el APK (todo desde el celu o la compu, sin instalar nada)

1. Creá una cuenta en https://github.com y un repositorio nuevo (ej: `huerta-de-lola`).
2. Subí **todo el contenido** de esta carpeta al repositorio (botón *Add file → Upload files*).
   Tiene que quedar la carpeta oculta `.github/workflows/build.yml` en el repo.
3. Entrá a la pestaña **Actions**. La compilación arranca sola (si no, elegí *Compilar APK → Run workflow*).
4. Cuando termine (unos 5-8 min), abrí esa ejecución y bajá **HuertaDeLola-APK** (está abajo, en *Artifacts*). Es un .zip con `app-debug.apk`.
5. Pasalo al celu, abrilo e instalalo (Android te va a pedir permitir "instalar apps desconocidas" para tu navegador o gestor de archivos).

## Si falla la compilación
Abrí el paso en rojo en la pestaña Actions, copiá el texto del error y mandámelo.

## Estructura
- `www/index.html`: el juego completo.
- `capacitor.config.json` y `package.json`: empaquetan el juego como app Android.
- `.github/workflows/build.yml`: receta que compila el APK.
