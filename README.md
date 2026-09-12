# mnkykonnekt-web

Web de una página de MNKY KONNEKT (https://mnkykonnekt.com). Hasta el 12/09/2026 servida en GitHub Pages desde `main`
(`CNAME` + `.nojekyll`); desde esa fecha el destino es **Cloudflare Pages** (GitHub Pages prohíbe el uso comercial), con
el DNS de Squarespace apuntando al proyecto de Pages cuando Miguel lo confirme.

**Rediseño «espectacular» (rama `espectacular`, 11-12/09/2026, dirección B «before → after theatre»):** `index.html`
llega del laboratorio `C:\dev\prospeccion-previews\lab\b\` con las rutas remapeadas (`img/`, `fonts/`, `demos/`,
`img/posters/`), sin `noindex` y con el beacon de Cloudflare Analytics. `demos/demo-*/` son las cuatro webs de negocios
ficticios (generadas por el motor de previews con `--final`, `noindex` a mano, sin datos marcables, `Disallow: /demos/`
en `robots.txt`); `img/posters/` sus pósters. Historia y decisiones: `C:\dev\prospeccion\docs\plans\2026-09-11-web-espectacular.md`
y `2026-09-12-web-tercera-vuelta.md`; auditoría en `lab\b\NOTAS.md` del laboratorio. **Desde el 12/09/2026 (noche) la web se edita directamente en este repo** (rama `espectacular`; Miguel hace el merge a `main`,
que es producción); el laboratorio `lab` queda como archivo y ya no se copia. Si hiciera falta volver a copiar desde el lab:
`sed` de `../assets/img/` → `img/`, `../assets/fonts/` → `fonts/`, `../pieces/posters/` → `img/posters/`, `../demos/` → `demos/`.

«Fast on a phone» en móvil (12/09, sesión dedicada, segunda vuelta tras el iPhone de Miguel): al llegar al 100 % del rail
**bajando y con el scroll en reposo** la página se ancla (`html.mkm-locked`) y solo se mueve la demo; se sale con la ×, la barra
«Back to MNKY» o Escape, que saltan la escena entera. El rail lleva una cola de 0,6 pantallas en la que la escena sigue completa
(la inercia que pasa de largo no se lleva la ×); subiendo desde abajo nunca se ancla y la demo no recibe el dedo: se entra tocando
el teléfono. Lecciones de iOS: `overflow: hidden` no frena el dedo y un `scrollTo` en plena inercia se ignora. Probado en Playwright
(390×844, con y sin `reduce`); el gesto real se comprueba en iPhone.

Desde el 2026-09-09 la página se **escribe a mano** en `index.html` (CSS y JS incrustados, GSAP por CDN con `defer`,
completa sin JavaScript y con `prefers-reduced-motion` respetado). Ya no se genera con el motor de previews:
es una pieza única con interacciones propias (antes/después arrastrable) y un enfoque de venta que el motor no
tiene. Qué se dice y por qué: `C:\dev\prospeccion\docs\archive\WEB-MNKY-ESTUDIO.md` (archivado; S3 reescribe la web).

- `mnky.json`: referencia histórica de textos y precios de la versión generada (2026-09-09, mañana). No se usa.
- `img/`: capturas **anonimizadas** (decisión de Miguel del 09/09, misma que LinkedIn; sector S0 del rework, 10/09):
  `before-salon` (web real con nombre y logo tapados), `after-salon` y `draft-<sector>` (previews construidas con un
  nombre genérico y teléfono `xxxx`). Ningún negocio real se nombra ni se enlaza desde esta web. Origen:
  `C:\MNKY\data\prospeccion\shots\linkedin\` y `shots\anon\`; variantes jpg/webp con Pillow.
- Precios: S$590 una vez · care plan opcional S$290/año desde el mes 13 (mensual a petición, no se publica) · .com.sg +S$79;
  sin bonus (S3, 11/09); fuente única `docs/OFERTA.md` del repo `prospeccion`. Contacto principal: WhatsApp `wa.me/34623827167`;
  email secundario. Pie con NIF, Registro Mercantil de Murcia y enlace al BORME (1/07/2025, asiento 296563); sin dirección
  social (D8, riesgo asumido). Bloque «Who you deal with» con Miguel Ángel López (foto pendiente de Miguel: `img/miguel.jpg`).
- Logo real (S3): `img/logo-{64,128,512}.{png,webp}` y favicons (`favicon-32/512.png`, `apple-touch-icon.png`) recortados con
  Pillow de `01 EMPRESA\Marca y Logo\LOGO MNKY KONNEKT.PNG`; `--brand #237A77` (teal del logo), `--paper #F9F6EF`, `--tint #F0EADE`.
- `privacy.html` indexable (desde el 10/09): contacto de protección de datos, baja = supresión, borrador 7 días.
- Contexto de negocio y decisiones: `C:\Users\hola\OneDrive\MNKY OS\Proyectos\Prospección IA.md`.
