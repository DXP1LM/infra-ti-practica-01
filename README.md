# Infraestructura de TI - Práctica 01

## Integrantes y roles
- Estudiante: DIEGO ALEXANDER LUQUE MAMANI. Rol inicial: demostrador.

## Caso Bodega El Barrio
Dos cajas y una PC de administracion usan un servicio de archivos, una aplicacion de inventario y un router.

## Componentes y funciones

- Componente: Router de red
  - Funcion: Conecta los equipos en red local (LAN) y gestiona el tráfico entre las cajas, la PC de administración y el servidor.
  - Si falla: Se interrumpe la comunicación total de la red; las cajas no pueden conectarse al servidor ni sincronizar el inventario.

- Componente: Servidor de archivos y aplicación de inventario
  - Funcion: Centraliza la base de datos de productos, almacena los documentos compartidos y procesa las peticiones de stock y ventas.
  - Si falla: Las cajas no pueden consultar existencias ni registrar ventas centralizadas; administración pierde acceso a los archivos compartidos.

- Componente: Terminales de punto de venta (Caja 1 y Caja 2)
  - Funcion: Registrar las transacciones de ventas diarias, procesar cobros y actualizar el inventario vendido en tiempo real.
  - Si falla: Se detiene la atención y cobro a clientes en esa estación de venta, generando demoras y pérdida de ingresos.

- Componente: PC de Administración
  - Funcion: Ejecutar tareas de gestión contable, supervisión de inventario, pedidos a proveedores y reportes del negocio.
  - Si falla: No se pueden emitir reportes gerenciales, registrar nuevas entradas de mercadería ni supervisar el estado financiero de la bodega.

## Lo aprendido
- Una idea nueva: La importancia de analizar el impacto de la falla de cada componente físico en la continuidad operativa del negocio.
- Una duda: ¿Cómo se implementa redundancia de red o respaldo automático en caso de caída del servidor principal?
