# NASA Space Apps · Managua

Landing page del NASA Space Apps Challenge Managua 2026, construida con Astro.

## Requisitos

- Node.js 20 o superior
- npm

## Ejecutar localmente

```bash
npm install
npm run dev
```

Luego abre [http://localhost:4321](http://localhost:4321).

## Comandos disponibles

```bash
npm run dev      # servidor de desarrollo
npm run check    # revisa errores de Astro y TypeScript
npm run build    # genera la versión de producción en dist/
npm run preview  # previsualiza la versión compilada
```

## Dónde modificar el proyecto

- `src/pages/index.astro`: contenido, enlaces, secciones, organizadores y contador.
- `src/styles/global.css`: colores, tipografías, layout, responsive y animaciones.
- `public/assets/`: flyers y logos utilizados por la página.

### Cambiar enlaces

Los enlaces principales están al inicio de `src/pages/index.astro`, dentro de `socials` y `officialUrl`.

### Cambiar el contador

La fecha objetivo está en el script de `src/pages/index.astro`:

```js
const target = new Date('2026-11-14T00:00:00-06:00').getTime();
```

El horario usa UTC-06:00, correspondiente a Managua.

## Flujo recomendado

Antes de subir cambios:

```bash
npm run check
npm run build
git add .
git commit -m "Describe el cambio"
git push
```

El proyecto genera un sitio estático y queda listo para hospedarse posteriormente en Vercel u otra plataforma compatible.
