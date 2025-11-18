# Modelo de dominio - Club Ocio SaaS (Backend)

## Roles de usuario

- SUPERADMIN:
  - Control total del sistema.
  - Puede gestionar admins y configuración global.
- ADMIN:
  - Gestiona usuarios (altas, bajas, inactivación).
  - Visualiza la actividad de usuarios.
- USER:
  - Usuario que disfruta de la plataforma según su membresía.

## Estados de usuario

- ACTIVE: puede autenticarse y usar la plataforma.
- INACTIVE: su cuenta existe pero no puede acceder.
- DELETED: cuenta eliminada definitivamente (solo referencia en logs si se decide).

## Entidades principales (nivel API)

- Usuario
- Rol
- Membresía
- Actividad
- Registro de actividad (logs)

Estas entidades se mapearán a tablas SQL en el futuro.
