# mnkykonnekt-web

Web de una página de MNKY KONNEKT SL (`mnkykonnekt.com`), servida en GitHub Pages desde `main`.

- **No se edita `index.html` a mano.** Se genera con el motor de previews de Prospección IA:
  `cd C:\dev\prospeccion; python prospeccion.py preview build --json C:\dev\mnkykonnekt-web\mnky.json --out C:\dev\mnkykonnekt-web\index.html --final`
- Textos, precios y muestras: `mnky.json`. Capturas de muestra: `img/` (se regeneran desde las previews con `--final`).
- Dominio: archivo `CNAME` (se añade cuando el DNS apunta a GitHub Pages; ver la ficha).
- Contexto de negocio y decisiones: `C:\Users\hola\OneDrive\MNKY OS\Proyectos\Prospección IA.md` (decisión 8, web propia).
