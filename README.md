# mnkykonnekt-web

Web de una página de MNKY KONNEKT (https://mnkykonnekt.com), servida en GitHub Pages desde `main` (`CNAME` + `.nojekyll`).

Desde el 2026-09-09 la página se **escribe a mano** en `index.html` (CSS y JS incrustados, GSAP por CDN con `defer`,
completa sin JavaScript y con `prefers-reduced-motion` respetado). Ya no se genera con el motor de previews:
es una pieza única con interacciones propias (antes/después arrastrable) y un enfoque de venta que el motor no
tiene. Qué se dice y por qué: `C:\dev\prospeccion\docs\WEB-MNKY-ESTUDIO.md`.

- `mnky.json`: referencia histórica de textos y precios de la versión generada (2026-09-09, mañana). No se usa.
- `img/`: capturas de las muestras (`draft-<slug>.jpg`, `after-the-parlour.jpg`) y de la web real del negocio del
  antes/después (`before-the-parlour.jpg`). Se regeneran con Playwright desde `C:\MNKY\data\prospeccion\shots\`.
- Precios: S$590 una vez · care plan S$29/mes · Google Business Profile S$199/mes. Contacto: hola@mnkykonnekt.com.
  Pie con NIF; sin dirección social por decisión de Miguel (LSSI art. 10 pendiente).
- Contexto de negocio y decisiones: `C:\Users\hola\OneDrive\MNKY OS\Proyectos\Prospección IA.md`.
