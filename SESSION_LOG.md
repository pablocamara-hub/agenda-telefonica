# Diario de sesiones

## Sesión 1 - AAAA-MM-DD
### Objetivo
Preparar la estructura y la memoria del proyecto.

### Realizado
- Creadas las carpetas y plantillas iniciales.

### Comprobaciones
- Nota: `hola.py` citado aquí no existe en el repo. Se descarta, el programa es `src/agenda.py`.

### Pendiente
- Inicializar Git y crear el plan de la versión 1.

### Primer paso de la próxima sesión
Leer README, AGENTS y TODO; después solicitar un plan sin programar.

## Sesión 2 - 2026-10-07
### Objetivo
Resolver incoherencias e implementar la v1 aprobada.

### Realizado
- Limpieza de `AGENTS.md` (plantilla pegada), `README.md` con validaciones y formato `nombre;telefono`.
- Renombrado `requeriments.txt` a `requirements.txt` (solo `pytest`). `.gitignore` sin `xlsx`.
- Creados `src/agenda.py`, `tests/test_agenda.py` y `data/contactos_ejemplo.txt`.
- `.claude/rules/CLAUDE.md` y `.github/copilot-instructions.md` apuntan a `AGENTS.md`.

### Comprobaciones
- Import y prueba manual de `src.agenda` OK con `python3`.
- `pytest` no disponible en este equipo (sin `pip3`). Pendiente de ejecutar.

### Pendiente
- Instalar `pytest` y ejecutar las 9 pruebas. Primer commit Git.

## Sesión 3 - 2026-10-13 (rama con-excel)
### Objetivo
Mismo programa, pero guardando en hoja de cálculo con `openpyxl`.

### Realizado
- Creado `.venv` local con `pip` y librerías `openpyxl` + `pytest` solo dentro del proyecto.
- Migrado `src/agenda.py`: constantes `RUTA_DATOS=data/contactos.xlsx`, `NOMBRE_HOJA=Contactos`.
- `cargar_contactos` lee filas desde la 2, ignora nombre vacío o teléfono no válido.
- `guardar_contactos` escribe cabecera `Nombre/Telefono` y teléfonos como texto.
- `requirements.txt` con `pytest` + `openpyxl` (justificado: Python no lee `.xlsx` solo).
- `tests/test_agenda.py`: 10 pruebas (7 de lógica + guardar/cargar + cabecera + filas malas).
- `.gitignore` ignora `data/contactos.xlsx`. `README.md`, `TODO.md`, `CHANGELOG.md` actualizados.

### Comprobaciones
- `.venv/bin/python -m pytest -q`: 10 passed.
- `guardar_contactos` + `cargar_contactos` con `data/contactos_ejemplo.xlsx`: OK (Ana, Luis).

### Pendiente
- Ninguno en esta rama. `main` sigue intacto con `.txt`.

