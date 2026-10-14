# Agenda Telefónica

## Objetivo
Crear una aplicación de consola en Python para gestionar contactos.

## Funcionalidades de la versión 1
- Añadir contactos (nombre y teléfono).
- Buscar contactos por nombre (parcial, sin distinguir mayúsculas).
- Buscar contactos por número (parcial o exacta).
- Eliminar contactos por nombre exacto, con confirmación `s/n`.
- Mostrar todos los contactos en orden alfabético (A-Z, sin distinguir mayúsculas).
- Mostrar todos los contactos en orden alfabético inverso (Z-A).
- Guardar y cargar contactos automáticamente desde una hoja de cálculo.

## Reglas de validación
- El nombre no puede estar vacío.
- El teléfono no puede estar vacío. Acepta dígitos, espacios, `+` y `-`.
- No se permiten dos contactos con el mismo nombre exacto.

## Formato de datos
- Fichero: `data/contactos.xlsx` (rama `con-excel`).
- Hoja `Contactos`, cabecera `A1=Nombre | B1=Telefono`.
- Desde la fila 2: un contacto por fila.
- Ejemplo: fila `Ana | 612345678`.
- Los teléfonos se guardan como texto para no perder `+` ni ceros.
- Si el fichero no existe, se empieza con agenda vacía.
- Si una fila tiene nombre vacío o teléfono no válido, se ignora y se avisa.

## Restricciones didácticas
- Programación estructurada.
- Funciones pequeñas y nombres descriptivos.
- Sin clases, sin bases de datos y sin decoradores en la versión 1.
- Código comprensible para alumnado de 2.º de Bachillerato.

## Estructura
- `src/`: código del programa (`src/agenda.py`).
- `tests/`: pruebas automáticas.
- `data/`: datos de ejecución (`contactos.xlsx` ignorado, `contactos_ejemplo.xlsx` de ejemplo).
- `docs/`: documentación adicional.

## Ejecución
```bash
python -m src.agenda
```

## Pruebas
```bash
pytest
```
- Necesita `pytest` y `openpyxl` (ver `requirements.txt`).
- Usa el entorno local: `.venv/bin/python -m pytest`.
