# Proyecto: Base de Datos - Centro Médico
Una Base de Datos SQL Server diseñada para demostrar mis habilidades en la creación, gestión y manipulación de bases de datos. Incluye scripts SQL para la creación de tablas, inserción de datos, consultas, procedimientos almacenados, vistas y más. Perfecto para mostrar competencias prácticas en SQL Server y T-SQL.


## Contenidos

- `CentroMedico.bak`: Archivo de copia de seguridad de SQL Server.
- `CentroMedico_script.sql`: Script SQL para crear la estructura y los datos de la base de datos.

## Conceptos Aplicados en la Base de Datos

### Implementación Inicial
- Creación de la base de datos manualmente y usando T-SQL.
- Creación de tablas y aplicación de Primary Key.
- Activación de la propiedad Identity.
- Definición de Foreign Keys con T-SQL.
- Creación de tablas relacionadas y tipos de datos de usuario.
- Diseño del "Modelo Entidad Relación" (DER).

### Manipulación de Registros DML
- SELECT y INSERT simple y multiple desde el entorno y con Query.
- Comandos UPDATE y DELETE.

### Sentencias DDL
- ALTER TABLE, ALTER COLUMN, DROP COLUMN, CREATE TABLE, DROP TABLE, TRUNCATE.

### Cláusulas SQL
- TOP, ORDER BY, DISTINCT, GROUP BY, WHERE.

### Funciones de Agregado
- MAX, MIN, SUM, AVG, COUNT, HAVING.

### Operadores Lógicos
- AND, OR, IN, LIKE, NOT, BETWEEN.

### Estructuras de Control
- IF ELSE, BEGIN END, EXISTS, WHILE, CASE, RETURN, BREAK, TRY CATCH.

### Operadores Aritméticos y de Comparación
- Suma, Resta, División, Multiplicación, Módulo.
- Comparación: Mayor o Igual, Menor o Igual, Distinto.

### Stored Procedures, Variables y Consultas
- Estructura, manipulación y uso de ANSI_NULLS en Stored Procedures.
- Declaraciones y asignaciones de variables, uso de ISNULL.

### Stored Procedures de Inserción, Consulta, Actualización y Eliminación
- Inserción de Pacientes, Turnos, TurnoPaciente, Médicos y MedicoEspecialidad.
- Obtención de Turnos de Paciente, Historia Clínica, Especialidades.
- Actualización de Turno y Paciente.
- Eliminación de Turno.

### Funciones de Conversión y Texto
- LEFT, RIGHT, LEN, LOWER, UPPER, REPLACE, REPLICATE, LTRIM, RTRIM, CONCAT.
- Funciones de fecha: GETDATE, GETUTCDATE, DATEADD, DATEDIFF, DATEPART, ISDATE.
- CAST y CONVERT.

### JOINS y UNIONS
- INNER JOIN, LEFT JOIN, RIGHT JOIN, UNION, UNION ALL.

### Transacciones
- BEGIN TRAN.

### Funciones Definidas por el Usuario
- Funciones escalares y de tabla.

### Tablas Temporales
- Tablas temporales en memoria y físicas.

### Vistas
- Creación y uso de vistas.

### Triggers
- Creación de Triggers de tipo INSERT y UPDATE.

### Scheduled JOBS
- Creación y configuración de SQL JOBS, emulación de Scheduled JOBS en SQL Server Express.

### Funciones, Scheduled Jobs y Vistas
- Función para convertir fecha a texto.
- JOB para cancelar turnos vencidos.
- Vista de médicos y especialidades.

### Administración de Usuarios, Roles, Schemas y Permisos
- Creación de usuarios, roles, asignación de roles, definición de schemas.

### Importación de Registros mediante Excel (Datos del Backup)
- Importación de registros desde hojas de cálculo y su impacto en la base de datos.

### Herramientas Adicionales
- SP_HELPTEXT, Shortcuts en la consola.

## Restaurar la Base de Datos

### Usando el archivo .bak

1. Abre SQL Server Management Studio (SSMS).
2. Conéctate a tu servidor de SQL Server.
3. Haz clic derecho en `Databases` > `Restore Database...`.
4. Selecciona `Device` y elige el archivo `CentroMedico.bak`.
5. Sigue las instrucciones para restaurar la base de datos.

### Usando el archivo .sql

1. Abre SQL Server Management Studio (SSMS).
2. Conéctate a tu servidor de SQL Server.
3. Abre una nueva `Query`.
4. En el menú superior, selecciona Query -> SQLCMD Mode para habilitar SQLCMD Mode.
5. Copia y pega el contenido de `CentroMedico_script.sql` en la `Query`.
6. Ejecuta el script para crear la base de datos.