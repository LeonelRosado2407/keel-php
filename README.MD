# Keel

Framework PHP construido desde cero sobre Slim4 — sin abstracciones de
terceros para el contenedor de dependencias, el sistema de migraciones,
seeders, Schema/Blueprint o el mecanismo de roles/permisos.

## Instalación en un proyecto

```bash
composer config repositories.keel vcs https://github.com/LeonelRosado2407/keel-php.git
composer require leonel/keel:^0.1
```

## Qué incluye

- Contenedor DI (PHP-DI) y capa de `Settings`/`config.php` fail-fast
- Migrator (batches, up/down/rollback/status) + Schema/Blueprint (CREATE y ALTER TABLE)
- `Seeder` base (Faker)
- `JwtService` (emisión/verificación de JWT)
- Mecanismo de roles/permisos: `AuthorizationService`, `RequiresPermission`,
  `PermissionRepositoryInterface`/`PermissionRepository`
- `ErrorHandler` PSR-15, `LoggerFactory` (Monolog)

## Comandos

```bash
composer test    # PHPUnit
composer stan     # PHPStan
composer migrate  # Migrator CLI
```

## Documentación

Wiki: https://github.com/LeonelRosado2407/keel-php/wiki
