# Hello SQL

# ¿Qué es una base de datos?

Una `base de datos` es un sistema organizado para almacenar, gestionar y recuperar información de forma eficiente, segura y consistente.

Características clave:

- Persistencia de los datos
- Acceso concurrente
- Integridad y consistencia
- Seguridad
- Escalabilidad

En SQL trabajamos con bases de datos relacionales, basadas en tablas relacionadas entre sí.

## ¿Qué es el modelo relacional?

El `modelo relacional` es un modelo matemático y lógico propuesto por Edgar F. Codd que organiza los datos en relaciones (tablas).

Principios básicos:

- Los datos se almacenan en tablas
- Cada tabla representa una entidad
- Las tablas se relacionan entre sí mediante claves
- Se evita la duplicidad innecesaria de datos
- Se garantiza la integridad de la información

# Elementos fundamentales del modelo relacional
## Tabla (Relación)

Estructura formada por:

- Filas (registros o tuplas) → datos individuales
- Columnas (atributos o campos) → características del dato

## Registro (Fila)

Representa una instancia concreta de la entidad.


## Campo (Columna)

Representa una propiedad específica del objeto.

Cada campo tiene:

- Tipo de dato
- Restricciones

Significado lógico

# Claves en bases de datos relacionales
## Clave primaria (PRIMARY KEY)

Identifica de forma única cada registro

- No puede ser NULL
- No puede repetirse
- Debe ser estable


### Buenas prácticas:

- Usar claves artificiales (id)
- Evitar datos “reales” como DNI o email como PK

## Clave foránea (FOREIGN KEY)

- Crea la relación entre tablas
- Apunta a la clave primaria de otra tabla
- Garantiza integridad referencial


# Relaciones entre tablas
🔹 Relación 1 a 1 (1:1)

Un registro de una tabla se relaciona con uno solo de otra.

Uso poco frecuente (normalmente por seguridad o separación lógica).

🔹 Relación 1 a N (1:N)

Un registro puede relacionarse con muchos registros de otra tabla.

Es la relación más común.

🔹 Relación N a M (N:M)

Muchos registros de una tabla con muchos de otra.

# Integridad de los datos
🔹 Integridad de entidad

Cada tabla debe tener una clave primaria.

La PK no puede ser NULL

🔹 Integridad referencial

Una FK debe apuntar a un registro existente.


🔹 Integridad de dominio

Los datos deben cumplir reglas:

- Tipo
- Longitud
- Rango
- Valores permitidos


# Normalización de bases de datos

La normalización es el proceso de organizar los datos para:

- Evitar duplicidades
- Reducir inconsistencias
- Facilitar mantenimiento

# Formas normales (resumen)

-  1FN: valores atómicos, sin listas
-  2FN: dependencia completa de la PK
-  3FN: sin dependencias transitivas



# ¿Qué es SQL?

SQL (Structured Query Language) es el lenguaje estándar para:

- Crear estructuras
- Insertar datos
- Consultar información
- Modificar registros
- Administrar bases de datos

SQL no es un lenguaje de programación, es un lenguaje declarativo.

# Tipos de comandos SQL

- DDL → estructura
- DML → datos
- DQL → consultas
- DCL → permisos
- TCL → transacciones

