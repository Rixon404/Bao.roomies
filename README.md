 Flujo de Uso Diario:
1. Tú creas/editas tareas → Auto-sync a GitHub (500ms delay)
2. Los otros abren la app → Auto-sync desde GitHub al cargar
3. Alguien completa tarea → Auto-sync a GitHub
4. Todos ven los cambios sin hacer nada manual


Como funciona la BD

┌─────────────────────────────────────────────────────────┐
│  Tú (Admin) creas las tareas en tu teléfono             │
│         ↓                                               │
│  La app guarda automáticamente en GitHub Repo           │
│  (archivo: bao-data.json)                               │
│         ↓                                               │
│  Los otros 3 abren la app → Leen de GitHub              │
│  ¡Datos sincronizados sin VPN!                          │
└─────────────────────────────────────────────────────────┘

RESUMEN DE CONFIGURACIÓN
Paso 1 Crear PAT en GitHub, Tú (Admin)
	 2 Crear bao-data.json en el repo, Tú (Admin)
     3 Configurar usuario/token en la app, Tú (Admin)
     4 Subir index.html actualizado a GitHub, Tú (Admin)
     5 Los otros 3 abren la web, Todos
     6 La app lee datos automáticamente, Automático