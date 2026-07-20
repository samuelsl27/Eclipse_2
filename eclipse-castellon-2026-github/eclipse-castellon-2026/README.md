# Eclipse total de sol — 12 de agosto de 2026 — Castellón

Mapa interactivo que muestra, minuto a minuto (20:00–21:00, cada 5 min), desde qué
zonas de la provincia de Castellón se verá el sol durante el eclipse total, teniendo
en cuenta las sombras del relieve (el sol estará a solo 4° de altura en el máximo).

**Datos:** MDT de 5 m del IGN (servicio WCS), efemérides DE421.
Sombras proyectadas calculadas con la altura y azimut reales del sol en cada instante.
Totalidad en Castellón capital: 20:31:19 – 20:32:54 (hora peninsular).

## Cómo publicarlo gratis en GitHub Pages

1. Crea una cuenta en [github.com](https://github.com) si no la tienes.
2. Pulsa **New repository**, llámalo por ejemplo `eclipse-castellon-2026`,
   déjalo **Public** y créalo.
3. En la página del repositorio pulsa **uploading an existing file**
   (o **Add file → Upload files**).
4. Arrastra TODO el contenido de esta carpeta: `index.html`, `README.md`,
   `.nojekyll` y la carpeta `img` con los 13 `.webp`
   (si arrastras la carpeta entera, GitHub respeta la estructura).
5. Pulsa **Commit changes**.
6. Ve a **Settings → Pages** y en *Build and deployment*:
   - Source: **Deploy from a branch**
   - Branch: **main** / carpeta **/ (root)** → **Save**
7. Espera 1-2 minutos. Tu web quedará en:
   `https://TU_USUARIO.github.io/eclipse-castellon-2026/`

Comparte esa URL con quien quieras.

## Notas

- La página es autocontenida (Leaflet va incrustado); solo necesita internet
  para el fondo de Google Maps.
- El fondo usa los tiles públicos de Google (`mt1.google.com`), que no son un
  servicio oficialmente soportado para webs de terceros. Para un uso serio,
  sustituye la URL del `L.tileLayer` en `index.html` por la API oficial de
  Google Maps o por Esri World Imagery:
  `https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}`
