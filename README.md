# Caso de Estudio: Lea$e ( again )

## Entregables
- [Diagrama de arquitectura](https://excalidraw.com/#room=15ad521ced3e2a893d54,jc9er6kXl3DlzgXnLj6XvA)
- [Video](https://drive.google.com/drive/folders/1yfok3g5Lus5d_C75p9fAYP3lO3qps6Qm?usp=sharing)

## REQUERIMIENTOS DEL SISTEMA

### Requerimientos funcionales

- Registro y validación de la empresa cliente
    1. Registro de la empresa cliente con los datos de RUC y razón social.
    2. Validación del estado activo y habido de la empresa en SUNAT.
    3. Consulta del historial crediticio de la empresa solicitante.
    4. Notificación de rechazo del registro por incumplimiento de las validaciones.
    5. Almacenamiento del perfil validado de la empresa cliente.
- Creación y evaluación inicial de la solicitud de compra
    1. Creación de la solicitud de compra por parte de la empresa cliente.
    2. Validación rápida de la disponibilidad de proveedores para los productos solicitados.
    3. Validación rápida de la capacidad financiera para costear la orden.
    4. Generación de un contrato preliminar de pre aprobación para la empresa cliente.
    5. Notificación al cliente con el contrato preliminar y el estado estimado de la operación.
    6. Generación de un ranking de proveedores candidatos según su orden de idoneidad.
- Evaluación y aprobación interna
    1. Aprobación de la orden de compra por parte del Gerente de Ventas.
    2. Evaluación de las condiciones y los plazos de entrega por parte del Gerente de Logística.
    3. Cálculo de las cuotas y del plan de cobro al cliente por parte del Gerente de Finanzas.
    4. Consolidación del plan de compra, entrega y financiamiento en un expediente interno.
- Contratación y aceptación del cliente
    1. Generación del contrato definitivo con las condiciones de pago, los plazos de entrega y el proveedor seleccionado.
    2. Envío del contrato definitivo a la empresa cliente para su revisión.
    3. Registro de la aceptación o el rechazo del contrato por parte del cliente.
- Activación de la orden y coordinación de la entrega
    1. Activación de la orden de compra al proveedor después de la aceptación del cliente.
    2. Programación de la fecha y las condiciones de entrega con el proveedor.
    3. Notificación a la empresa cliente de la fecha de entrega confirmada.
- Entrega y conformidad
    1. Registro del acta de entrega y conformidad firmada por el cliente.
    2. Verificación, por parte del cliente, del estado de los insumos recibidos dentro de una ventana de
    48 horas.
    3. Registro de las observaciones o los defectos reportados por el cliente después de la entrega.
- Gestión de incidencias e incumplimientos
    1. Notificación automática al cliente ante un atraso confirmado en la entrega.
    2. Registro y clasificación del tipo de incidencia: Atraso, Producto incorrecto y Daño durante el tránsito.
    3. Aplicación de una penalidad escalonada al proveedor según los días de retraso.
    4. Gestión del reemplazo o reenvío del pedido ante el incumplimiento del proveedor.
    5. Transferencia de los derechos de garantía al cliente para que pueda realizar una reclamación
    directa al proveedor.
    6. Activación de la cláusula de fuerza mayor ante eventos no imputables al proveedor.
    7. Cancelación de la orden y reasignación a un proveedor alternativo por retraso crítico.

### Requerimientos no funcionales

1. Rendimiento: el tiempo de respuesta de las validaciones rápidas debe ser menor a 3 segundos.
2. Trazabilidad: el sistema debe proporcionar trazabilidad completa de cada solicitud, desde el
registro de la empresa hasta la entrega.
3. Notificaciones: el sistema debe enviar notificaciones por correo electrónico ante cada cambio de
estado del flujo.
4. Seguridad: el sistema debe contar con autenticación segura para el acceso de los gerentes al
sistema interno.
5. Auditoría: el sistema debe mantener un registro de auditoría de todas las aprobaciones y
decisiones realizadas durante el flujo.