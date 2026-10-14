 # Plan y tareas

## En curso (rama con-excel)
- [x] Crear `.venv` local e instalar `openpyxl` + `pytest` solo dentro del proyecto.
- [x] Migrar `src/agenda.py` a `data/contactos.xlsx` (hoja `Contactos`).
- [x] Actualizar `tests/test_agenda.py` a Excel (10 pruebas).
- [x] Ejecutar `.venv/bin/python -m pytest` y prueba manual.
- [x] Crear `data/contactos_ejemplo.xlsx` y hacer commit en `con-excel`.

## Pendientes
- [ ] Instalar `pytest` y ejecutar `tests/test_agenda.py` (no disponible en este equipo).

## Terminadas
- [x] Crear estructura inicial.
- [x] Redactar documentación básica.
- [x] Limpiar `AGENTS.md` y aclarar requisitos v1.
- [x] Definir formato del fichero (`nombre;telefono` en `data/contactos.txt`).
- [x] Crear el menú.
- [x] Añadir contactos (validar vacío y duplicado exacto).
- [x] Buscar contactos por nombre (parcial, sin mayúsculas).
- [x] Buscar contactos por número (parcial).
- [x] Eliminar contactos (nombre exacto + confirmación).
- [x] Mostrar contactos A-Z.
- [x] Mostrar contactos Z-A.
- [x] Guardar y cargar datos automáticamente.
- [x] Crear pruebas (`tests/test_agenda.py`, una por comportamiento).
- [x] Primer commit Git.


