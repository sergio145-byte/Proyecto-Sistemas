# Mi Dinero 💰

App para el teléfono que sirve para llevar el dinero del mes: ingresos, gastos, presupuesto por categoría y saldo.

Es una aplicación web instalable (PWA): se abre en el navegador del móvil, se añade a la pantalla de inicio y funciona sin conexión. Los datos se guardan **solo en tu teléfono**, en el almacenamiento del navegador.

## Qué hace

- **Resumen del mes:** saldo, ingresos, gastos y un gráfico de gastos por categoría.
- **Movimientos:** añadir, editar y eliminar gastos o ingresos, y buscarlos.
- **Movimientos que se repiten** (sueldo, alquiler…): marca "Repetir cada mes" y aparecerán solos cada mes.
- **Presupuesto:** un límite por categoría con barra de progreso (se pone naranja al llegar al 85 % y roja si te pasas).
- **Navegación por meses** con las flechas de arriba.
- **Ajustes:** moneda, categorías propias y copia de seguridad (exportar o importar en JSON y exportar el mes a CSV para Excel).
- Modo oscuro automático.

## Cómo ponerla en tu teléfono

1. Publica el repositorio con **GitHub Pages**: en GitHub ve a *Settings → Pages*, en *Branch* elige la rama y la carpeta `/ (root)`, y guarda.
2. Abre en el móvil la dirección que te da GitHub (`https://<usuario>.github.io/<repositorio>/`).
3. Instálala:
   - **Android (Chrome):** menú ⋮ → *Añadir a pantalla de inicio* o *Instalar app*.
   - **iPhone (Safari):** botón Compartir → *Añadir a pantalla de inicio*.

Para probarla en el ordenador: `python3 -m http.server` en esta carpeta y abre `http://localhost:8000`.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app entera (interfaz, estilos y lógica) |
| `manifest.json` | Nombre, icono y colores para instalarla |
| `sw.js` | Hace que funcione sin conexión |
| `icon.svg` | Icono de la app |

> ⚠️ Si borras los datos del navegador o cambias de teléfono, se pierden los datos. Usa **Ajustes → Exportar datos** de vez en cuando para tener una copia.
