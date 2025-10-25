# Gastos — iPhone App (HTML + LocalStorage)

App web estilo iOS para controlar gastos desde el móvil. Sin backend. Todos los datos viven en `localStorage` del navegador.

## Funciones
- Añadir gasto: nombre, importe, fecha, categoría, método de pago, notas.
- Marcar gasto recurrente (semanal o mensual). Se autogenera en el futuro.
- Configuración:
  - Categorías personalizadas.
  - Métodos de pago personalizados.
  - Presupuesto mensual y moneda.
  - Importar / exportar JSON.
  - Borrado total con advertencia.
- Histórico:
  - Lista de todos los gastos.
  - Editar o eliminar cada gasto.
  - Exportar CSV listo para Excel / Sheets.
  - Ordenar por fecha.
- Dashboard:
  - 5 KPIs clave del mes.
  - Gráfica de barras por categoría.
  - Línea con gasto semanal.
  - Doughnut de distribución.
  - Todo con Chart.js CDN.

## Persistencia
- Se guarda todo en `localStorage`, por lo que:
  - Cada dispositivo tiene sus propios datos.
  - No requiere servidor.
  - Al borrar datos o limpiar caché se pierde la información salvo que antes se exporte JSON.

## Avatar
- Puedes guardar una foto de perfil.
- La imagen se guarda en base64 en `localStorage`.

## Estructura del repo
```text
gastos-app/
  index.html
  README.md
  .gitignore
  css/
    style.css
  js/
    app.js
```

## Uso rápido
1. Abre `index.html` en el navegador del iPhone (Safari).
2. Añade a pantalla de inicio si quieres experiencia tipo app.
3. Empieza a meter gastos. Todo queda guardado.

## GitHub Pages
Si subes esta carpeta a GitHub como repo público y activas GitHub Pages, podrás usar la app desde la URL del repo directamente en el iPhone.

## Licencia
Este proyecto se puede usar y modificar libremente.
