# Historial de cambios

## [con-excel]
### Añadido
- Dependencia `openpyxl` en `requirements.txt` (necesaria para leer/escribir `.xlsx`).
- `tests/test_agenda.py`: 10 pruebas, con `test_guardar_crea_cabecera` nueva.
- Hoja `Contactos` con cabecera `Nombre | Telefono`.

### Cambiado
- `src/agenda.py`: `cargar_contactos` y `guardar_contactos` usan `data/contactos.xlsx`.
- Teléfonos guardados como texto para conservar `+` y ceros.
- `README.md`, `.gitignore` (`data/contactos.xlsx`) y `TODO.md` actualizados.
- `main` sigue con `.txt`; este cambio vive solo en `con-excel`.

## [Sin publicar]
### Añadido
- Estructura inicial del proyecto.
- Documentación de contexto y continuidad.
- `src/agenda.py`: menú, añadir, buscar por nombre/número, eliminar, mostrar A-Z/Z-A, guardar/cargar `nombre;telefono`.
- `tests/test_agenda.py`: 9 pruebas (validación, duplicado, búsquedas, eliminar, orden, guardar/cargar, líneas malas).
- `requirements.txt` solo con `pytest`. `data/contactos_ejemplo.txt` de ejemplo.

### Corregido
- `AGENTS.md` limpio y sin contradicciones con `README.md`.
- `README.md` con validaciones y formato de fichero.
- Eliminado `requeriments.txt` mal escrito y mezclado. `xlsx` fuera.

