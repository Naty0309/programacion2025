# Panel Ctas Ctes 2026

Aplicación web de una sola página para gestionar **cuentas corrientes** de clientes
(Ctas Ctes SC). Funciona sin conexión y sin servidor: abrís el archivo y listo.

## Cómo usarlo

Abrí `index.html` con doble clic (o desde tu navegador). No necesita internet ni instalación.

## Qué permite hacer

- **Clientes**: alta, edición y baja (nombre, teléfono, localidad, notas).
- **Movimientos** por cliente:
  - **Debe (cargo)**: lo que el cliente compra / se le factura.
  - **Haber (pago)**: lo que el cliente paga.
  - Saldo acumulado calculado automáticamente en cada línea.
- **Panel resumen**: cantidad de clientes, total a cobrar, clientes con deuda y saldo a favor.
- **Buscador** de clientes por nombre o localidad.
- **Imprimir** el estado de cuenta de un cliente (`🖨 Imprimir estado`).
- **Backup / Importar**: descargá un archivo `.json` con todos los datos y restauralo cuando quieras.

## Dónde se guardan los datos

Los datos se guardan en el **navegador** de la computadora (localStorage), en la clave
`panelCtasCtes2026`. Son locales a esa computadora y ese navegador.

> ⚠️ **Importante**: si borrás los datos del navegador, cambiás de equipo o de navegador,
> los datos no aparecen. Usá **Backup** seguido para no perder información y guardá el
> archivo `.json` en un lugar seguro (por ejemplo tu carpeta de la nube).

## Signo del saldo

- Saldo **positivo (rojo)** → el cliente **debe** dinero.
- Saldo **negativo (verde)** → el cliente tiene **saldo a favor** (pagó de más / anticipo).
- Saldo **cero** → cuenta saldada.
