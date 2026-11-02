# Tales of Darkness

Juego de supervivencia contra hordas con estética pixel art. Creas tu héroe (8 razas, versión masculina y femenina) y sobrevives en un mundo infinito de biomas mientras aprendes habilidades de 6 elementos, consigues equipo y desbloqueas cosméticos.

**Jugar:** https://jgutiero1993-rgb.github.io/tales-of-darkness/

Se puede instalar como app en Android, iPhone/iPad y PC, y funciona sin conexión.

## Características

- **Héroe personalizable:** sexo, raza, piel, peinado, color de pelo, barba y vestimenta.
- **170 habilidades:** 27 tipos de ataque (mágicos, a distancia y cuerpo a cuerpo) × 6 elementos, más 8 neutrales. Cada elemento aplica su efecto: Frío, Quemadura, Quebranto, Descarga, Purificación o Maldición.
- **Pack de hasta 16 habilidades:** 4 ranuras en partida que se vinculan en las grietas dimensionales.
- **Mejoras:** hasta 100 puntos repartidos en Ataque físico, Ataque especial, Vida, Defensas, Velocidad, Crítico y Recarga.
- **Equipo:** arma, casco, armadura, botas y amuleto, con rangos de C a SS.
- **Cosméticos:** 71 aspectos que nunca afectan al juego.
- **Altar de Invocación, tienda, misiones, logros y clasificación local.**

## Controles

- **PC:** `WASD` para moverte, `1`–`4` para elegir la ranura activa, `Q`/`E` para cambiar de ranura y `Esc` para pausar.
- **Móvil:** arrastra para moverte y toca una ranura para seleccionarla.
- **Mando:** stick izquierdo, `LB`/`RB` para cambiar de ranura y `Start` para pausar.

## Estructura

| Archivo | Para qué sirve |
|---|---|
| `index.html` | El juego completo (HTML, CSS y JavaScript en un solo archivo) |
| `manifest.webmanifest` | Datos de la app instalable: nombre, iconos, pantalla completa |
| `sw.js` | Service worker: juego sin conexión y actualizaciones automáticas |
| `icons/` | Iconos de la app y la imagen para compartir en redes |
| `.nojekyll` | Hace que GitHub Pages publique los archivos tal cual |
| `_headers` | Ajustes de caché si se publica en Netlify o Cloudflare Pages |

## Publicar cambios

Basta con subir el nuevo `index.html` (y los demás archivos si cambian) a la rama `main`: GitHub Pages lo publica en uno o dos minutos. Si cambias el juego, sube también la versión de la caché en `sw.js` (`VERSION`) para que quien tenga la app instalada reciba la actualización.

## Estado

Prototipo v0.5. El progreso se guarda en el navegador de cada dispositivo. Próximas fases: cuentas y guardado en la nube, multijugador cooperativo y tienda.
