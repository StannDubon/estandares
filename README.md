# Estándares de Enfermería (Flask + Postgres)
Local: `pip install -r requirements.txt && python -m flask --app app run` (usa SQLite; admin/cambiar123 si no defines ADMIN_USER/ADMIN_PASSWORD).
## Deploy gratis
1. **Neon** (neon.tech, gratis): crea un proyecto y copia el connection string -> `DATABASE_URL`.
2. Sube esta carpeta a un repo de GitHub.
3. **Render** (render.com, Web Service gratis): Build `pip install -r requirements.txt`, Start `gunicorn app:app`.
   Variables: `DATABASE_URL`, `SECRET_KEY` (texto largo aleatorio), `ADMIN_USER`, `ADMIN_PASSWORD`.
Nota: Render gratis se "duerme" tras 15 min sin uso (el primer acceso tarda ~1 min). Los datos viven en Neon, no se pierden.
