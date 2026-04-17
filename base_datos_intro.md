# 1. El rol de una base de datos
Una base de datos relacional actúa como el "cerebro logístico" de una organización. Su función principal no es solo guardar datos, sino estructurarlos y relacionarlos de forma que la información sea confiable, coherente y fácil de consultar. Permite que diferentes áreas de una empresa lean y escriban información simultáneamente sin que los datos se corrompan o se dupliquen innecesariamente.

3 ejemplos concretos de uso:

Sistema de Ventas y Facturación: Para registrar cada transacción, asociando un cliente específico con los productos comprados, el vendedor que realizó la operación y la fecha exacta.

Gestión de Recursos Humanos: Para mantener el historial de los empleados, sus salarios, departamentos y evaluaciones de desempeño, asegurando que cada contrato esté ligado a una persona única.

Control de Inventario en Tiempo Real: Para saber cuántas unidades quedan de un producto, quién es el proveedor de ese lote y generar alertas automáticas cuando el stock es bajo.

# 2. Características de un RDBMS
Un RDBMS (Relational Database Management System) es el software que sirve de interfaz entre el usuario y la base de datos física. Es el programa que realmente ejecuta las instrucciones SQL para crear, leer, actualizar o borrar datos.

3 características que lo diferencian:

Integridad Referencial: Garantiza que las relaciones entre tablas sean consistentes (por ejemplo, no puedes borrar un cliente si aún tiene facturas pendientes).

Cumplimiento de ACID: Asegura que las transacciones sean Atómicas, Consistentes, Aisladas y Duraderas; es decir, que si algo falla durante un proceso, el sistema vuelve al estado anterior para evitar errores.

Estructura mediante Esquemas: Los datos se organizan estrictamente en tablas con columnas y tipos de datos definidos antes de insertar la información.

3 RDBMS ampliamente usados:

PostgreSQL: Muy usado en aplicaciones web complejas y análisis de datos por su robustez y soporte de tipos de datos avanzados.

MySQL: El estándar para la mayoría de los sitios web y gestores de contenido (como WordPress) debido a su velocidad y facilidad de uso.

Microsoft SQL Server: Preferido en entornos corporativos que utilizan el ecosistema de Windows, ideal para grandes empresas que requieren soporte técnico dedicado y alta integración con herramientas de negocios.

# 3. Herramientas y objetos
Para interactuar con estas bases de datos, existen dos vías principales:

Herramientas Gráficas (GUI): Como DBeaver o pgAdmin, que permiten ver las tablas y datos de forma visual.

Línea de Comandos (CLI): Como el terminal de psql (para PostgreSQL) o el propio MySQL Shell, donde se escriben las sentencias directamente.

Objetos de una Base de Datos:
Tabla: Es la unidad básica de almacenamiento, organizada en filas (registros) y columnas (campos).

Vista: Una "tabla virtual" que muestra el resultado de una consulta guardada; no almacena datos propios, sino que facilita el acceso a información compleja de otras tablas.

Índice: Una estructura que acelera la búsqueda de datos (funciona como el índice de un libro, permitiendo encontrar información sin leer toda la tabla).

Llave primaria (Primary Key): Un campo único que identifica de forma irrepetible a cada registro dentro de una tabla (por ejemplo, el RUT o un ID de usuario).

Llave foránea (Foreign Key): Un campo que vincula una fila de una tabla con la llave primaria de otra, estableciendo la relación técnica entre ellas.