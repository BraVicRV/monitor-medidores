# Monitor de Medidores Inteligentes

Aplicación web estática (HTML + JavaScript). Todo el análisis se hace en el navegador:
los Excel NO se suben a ningún servidor.

## Funciones
- Carga de Excel por zona (13, 14, 15, 16) y mes, con verificación del nombre del archivo y del mes.
- Indicadores, tarjetas por zona (lecturados / no lecturados, promediados) y filtros.
- Gráficos 3D (interruptor para desactivarlos), incidencias por categoría con texto real.
- Tabla de medidores promediados y detalle de medidores.
- Descarga de reporte en PDF.

## Desplegar en Render (Static Site)
1. Sube esta carpeta a un repositorio de GitHub/GitLab.
2. En Render: New + > Static Site (o Blueprint, que lee `render.yaml`).
3. Si lo creas manualmente: Build Command vacío, Publish Directory = `public`.
4. Deploy. Render te dará una URL https://monitor-medidores.onrender.com (o similar).

## Notas
- Requiere internet en el navegador: las librerías (SheetJS, Chart.js, jsPDF) se cargan desde cdnjs.
- Para probar local: `cd public && python3 -m http.server 8000` y abrir http://localhost:8000
