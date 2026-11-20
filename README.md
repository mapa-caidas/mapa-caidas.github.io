# Mapa de Caídas

PWA sin servidor: pegas el aviso, ubica a los clientes por número de portal (CartoCiudad/IGN), agrupa por zonas y exporta para planta externa.

## Publicar (GitHub Pages)
1. Crea un repo (p. ej. `mapa-caidas`) y sube TODO el contenido de esta carpeta a la raíz.
2. Settings → Pages → Branch `main` / root → Save.
3. Abre `https://<usuario>.github.io/mapa-caidas/` en el móvil → menú ⋮ → «Instalar aplicación».

Tiene que ir por https (GitHub Pages ya lo da); abierto como archivo local no se instala ni da GPS.

## Actualizar
Sube los cambios y sube la versión en `sw.js` (`VERSION = 'caidas-v1.0.1'`) para que los móviles cojan la nueva.

## Datos
No se guarda nada fuera del móvil. La incidencia abierta queda en el navegador hasta pulsar «Nueva incidencia».
Geocodificación: CartoCiudad (IGN) y, si falla, OpenStreetMap/Nominatim. Mapas: IGN (callejero y ortofoto PNOA) y Esri.

## Probar sin publicar
Abre index.html con doble clic: lleva todo dentro. Instalarla como app requiere publicarla por https.

## Incidencias guardadas
Cada incidencia se guarda sola en el navegador (botón «📂 Guardadas»). «Nueva incidencia» guarda la actual y abre otra en blanco. El historial va ligado a la dirección de la app: instalada desde GitHub Pages se conserva; abriendo index.html con doble clic depende de la carpeta. Exporta el .json de las importantes.
