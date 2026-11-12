# Datos ficticios

Todos los datos del proyecto son inventados. No proceden de ninguna empresa real ni contienen información de personas reales.

Viven en tres tablas de Dataverse:

- **Clientes** — clientes ficticios con su centro asociado
- **Productos_Servicios** — audífonos y servicios del catálogo
- **Incidencias** — tabla principal (código `INC-0000`, tipo, prioridad, estado, escalado, canal, descripción, fechas, resolución, autor y propietario)

Las incidencias usadas para medir la clasificación (45 descripciones con su resultado esperado) están en [`../evaluacion/`](../evaluacion/), en CSV listo para *Importar desde CSV* en Dataverse y en Excel con los resultados.

Los valores internos de las columnas de opción (por ejemplo, Estado *Escalada* = `610150002`) están en las memorias técnicas de [`../docs/`](../docs/).
