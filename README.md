# mnkykonnekt-web

Web de una página de MNKY KONNEKT (https://mnkykonnekt.com), servida en GitHub Pages desde `main` (`CNAME` + `.nojekyll`).

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
