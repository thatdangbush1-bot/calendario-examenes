# Calendario de Exámenes · FP

Página de calendario para ver y añadir exámenes del curso (CFGS Sistemas microinformáticos y redes).

Publicada en GitHub Pages: **https://thatdangbush1-bot.github.io/calendario-examenes/**

## Cómo funciona

- Los exámenes "canónicos" viven en `data.js` (`window.EXAMS`).
- La página permite añadir/editar/borrar exámenes desde el navegador; esos cambios quedan en `localStorage` del navegador como "cambios locales".
- Para subir cambios a la web: botón **⬇ Exportar** → genera el `data.js` completo → descargar o copiar → guardarlo aquí y subirlo con git (o pedírselo a OpenCode).

## Gestionar con OpenCode

Desde local (sin abrir el navegador) se pueden tocar directamente los exámenes en `data.js` y luego:

```bash
git add data.js
git commit -m "Actualizar exámenes"
git push
```

## Estructura

- `index.html` — página completa (calendario + lista, estilos y lógica).
- `data.js` — datos de exámenes.