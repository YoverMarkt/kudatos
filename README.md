# Kudatos — Landing

Landing page estática de **Kudatos** (consulta de cédulas y placas del Ecuador).
Es 100% HTML/CSS/JS: `index.html` + la carpeta `assets/` (runtime JS y fuentes Inter).

## Ver en local

```bash
npm start          # servidor en http://localhost:3000
# o cualquier servidor estático:
npx serve .
```

## Despliegue

### GitHub Pages
Se sirve directamente desde la raíz del repo. El archivo `.nojekyll` evita que
Jekyll ignore la carpeta `assets/`.

### Railway
Railway usa `package.json` → `npm start` → `server.js`, un servidor estático
mínimo que escucha en `process.env.PORT`.

## Estructura

```
index.html          Página (usa un runtime propio embebido en assets/*.js)
assets/             Runtime JS + fuentes woff2
server.js           Servidor estático para Railway
package.json        Script de arranque
.nojekyll           Config GitHub Pages
source/             Archivo original empaquetado (referencia)
```
