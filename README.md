# Cuervo Lighting Designer Studio — Sitio + Panel de edición

## Qué hay en esta carpeta
- `index.html` — el sitio público (igual que antes, con todo el diseño y animaciones).
- `content/clients.json` y `content/projects.json` — las listas de clientes y proyectos. El sitio las lee de aquí; el panel de edición las modifica aquí.
- `admin/` — el panel de edición (Decap CMS). Solo tú (o quien invites) puede entrar.
- `images/uploads/` — aquí se guardan las fotos que subas desde el panel.

## Paso 1 — Subir esto a GitHub
1. Crea un repositorio nuevo en GitHub (puede ser privado), por ejemplo `cuervo-lighting-site`.
2. Sube TODO el contenido de esta carpeta a ese repositorio (arrastrando los archivos en la web de GitHub, o con `git push` si prefieres terminal).

## Paso 2 — Reconectar Netlify a ese repositorio
1. En Netlify, ve a tu sitio actual → **Site configuration** → **Build & deploy**.
2. Busca la opción de **"Link repository"** o crea el sitio de nuevo con **"Import from Git"** apuntando al repo que acabas de crear.
3. No necesitas configurar ningún build command — es un sitio estático, se publica tal cual.

## Paso 3 — Activar Netlify Identity
1. En tu sitio dentro de Netlify → pestaña **"Identity"** → **"Enable Identity"**.
2. Baja a **"Registration"** → cámbialo a **"Invite only"** (así nadie se registra solo).
3. Baja a **"Services"** → **"Git Gateway"** → **"Enable Git Gateway"** (esto es lo que le da permiso al panel de editar el repositorio por ti).

## Paso 4 — Invitarte a ti mismo
1. Sigue en la pestaña **"Identity"** → botón **"Invite users"**.
2. Pon tu correo (o el de quien más quieras que edite).
3. Te va a llegar un correo de invitación — ahí defines tu contraseña.

## Paso 5 — Entrar a editar
1. Ve a `tusitio.com/admin` (el dominio real que te da Netlify o el tuyo propio).
2. Inicia sesión con el correo/contraseña que configuraste.
3. Ahí puedes:
   - Editar la lista de **Clientes** (nombre + foto).
   - Editar la lista de **Proyectos** (nombre, tipo, ubicación, año + foto).
4. Cada "Publish" que hagas actualiza el sitio real en 1-2 minutos.

## Nota
Los visitantes normales del sitio (tus clientes) **nunca ven ni necesitan** el `/admin` — ese link nomás lo conoces tú.
