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
- **Evoluciones:** cada habilidad a nivel 5 evoluciona si llevas la mejora pasiva que le corresponde.
- **Combos de elementos:** vincular habilidades de elementos distintos provoca 15 reacciones (Vapor, Magma, Tormenta…).
- **Compañeros:** 6 criaturas, una por elemento, que salen de huevos, luchan a tu lado y evolucionan en la partida.
- **Actos y jefes:** Acto I con 6 fases y 5 jefes hasta el Rey Caído; Acto II con demonios, lluvia de azufre y el Rey Demonio; después, el Abismo Eterno.
- **Biomas vivos:** enemigos propios de cada bioma, un guardián por bioma y élites con afijos (veloces, explosivos o con escudo elemental).
- **Altares y esencias:** altares que dan bendiciones de 30 s y esferas de esencia de 5 colores.
- **Cooperativo hasta 4 jugadores** con salas por código, invitaciones y lista de amigos, y **Duelo 1 contra 1** al mejor de tres asaltos con tus 16 habilidades en 4 vínculos de 4.
- **Música** propia para cada bioma, los jefes y las grietas.
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

Prototipo v0.6. El progreso se guarda en el navegador de cada dispositivo. El cooperativo y el duelo conectan los navegadores directamente (PeerJS), así que necesitan internet. Próximas fases: clasificación en línea, cuentas y guardado en la nube, y tienda.
