# Modelo de datos inicial

## Entidades

### `personas`
- `id` (PK)
- `nombres`
- `apellidos`
- `sexo_genero_id` (FK)
- `tipo_discapacidad_id` (FK)
- `direccion`
- `region_id` (FK)
- `municipio`
- `telefono`
- `estado_id` (FK)
- `observaciones`
- `created_at`
- `updated_at`

### `cat_tipos_discapacidad`
- `id` (PK)
- `nombre`
- `activo`

### `cat_sexo_genero`
- `id` (PK)
- `nombre`
- `activo`

### `cat_regiones`
- `id` (PK)
- `nombre`
- `activo`

### `cat_estado_registro`
- `id` (PK)
- `nombre` (activo/inactivo)

### `usuarios`
- `id` (PK)
- `nombre`
- `email`
- `password_hash`
- `rol` (admin, operador, consulta)
- `activo`

## Reglas de integridad

- Todos los FKs deben validar contra catálogos activos.
- `nombres`, `apellidos`, `tipo_discapacidad_id`, `sexo_genero_id`, `direccion`, `region_id` son obligatorios.
- `created_at` y `updated_at` se gestionan automáticamente.
