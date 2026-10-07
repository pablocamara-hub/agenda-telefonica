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

