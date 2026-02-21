# Requisitos funcionales MVP

## 1) Registro de persona atendida

Campos mínimos:
- `nombres` (obligatorio)
- `apellidos` (obligatorio)
- `tipo_discapacidad` (obligatorio, catálogo)
- `sexo_genero` (obligatorio, catálogo)
- `direccion` (obligatorio)
- `region` (obligatorio, catálogo)
- `municipio` (opcional)
- `telefono` (opcional)
- `fecha_registro` (automática)
- `estado` (activo/inactivo)
- `observaciones` (opcional)

## 2) Búsqueda y filtros

El sistema debe permitir:
- Buscar por nombre y apellido.
- Filtrar por región.
- Filtrar por tipo de discapacidad.
- Filtrar por estado (activo/inactivo).

## 3) Edición y mantenimiento

El sistema debe permitir:
- Editar datos de contacto y ubicación.
- Actualizar estado del registro.
- Mantener historial básico de última actualización.

## 4) Seguridad mínima

- Acceso autenticado por usuario.
- Roles mínimos:
  - Administrador
  - Operador
  - Consulta
