# SEEDER

<BR>

### Código Fuente✅
El código del seeder lo podemos encontrar dentro de esta url: https://github.com/Alex01Dev/backend-cc/blob/main/seed/seed.py
<BR>

### Respaldo de la BD Vacía (Sin datos Generados)✅
Archivo de la estructura de la bd que puede ser relacional o no relacional.
<BR>

### Listado de EndPoint para Generar datos simulados✅
Tabla que contendrá los endpoint y descripción de la funcionalidad sobre los datos.

| Endpoint                     | Método | Descripción                                                                 |
|------------------------------|--------|-----------------------------------------------------------------------------|
| `/Backend_cc/seed/seed.py/Usuarios`            | POST   | Genera usuarios simulados con nombre, correo, contraseña e imagen de perfil. |
| `/Backend_cc/seed/seed.py/Productos`         | POST   | Genera productos ecológicos ficticios con nombre, descripción, precio e imagen. |
| `/Backend_cc/seed/seed.py/Comentarios`         | POST   | Crea comentarios de prueba asociados a usuarios y productos.                |
| `/Backend_cc/seed/seed.py/Interacciones`     | POST   | Genera interacciones simuladas (likes, valoraciones) entre usuarios y productos. |
| `/Backend_cc/seed/seed.py/Cart`     | POST   | Crea transacciones financieras ficticias entre usuarios y productos.        |
| `/Backend_cc/seed/seed.py/Purchase`              | POST   | Crea datos simulados pasando los de cart a purchease, simulando la comrpa de un usuario. |
<BR>

### Screenshots (Capturas de Pantall)✅
De los Endpoint que generan los datos
<BR>

### Respaldo de la BD Post Llenado (1,000,000 de registros)✅
Respaldo de la base de datos ya con datos generados mismos que servirán para alimentar los algoritmos de análisis supervisado y no supervisado