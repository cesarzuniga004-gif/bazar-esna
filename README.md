# Bazar El Tiburón — Página de Prendas

Sitio estático (HTML/CSS/JS puro, sin frameworks) pensado para publicarse
gratis en **GitHub Pages**. La vista pública solo muestra el catálogo; el
modo administrador (🔒 arriba a la derecha) permite editar nombres,
precios, tallas y subir fotos — los cambios se guardan directo en este
repositorio de GitHub y se publican automáticamente en 30 segundos a 2
minutos.

## 1. Crea el repositorio

1. Entra a [github.com](https://github.com) e inicia sesión (o crea una
   cuenta gratis).
2. Arriba a la derecha, clic en **+** → **New repository**.
3. Nómbralo, por ejemplo `bazar-tiburon`. Déjalo **Public** (para que
   GitHub Pages sea gratis). Crea el repositorio.

## 2. Sube estos archivos

1. Dentro del repositorio recién creado, clic en **Add file** →
   **Upload files**.
2. Arrastra **todo el contenido de esta carpeta** (el archivo
   `index.html`, este `README.md` y la carpeta `data/` completa, con
   `data/prendas.json` adentro). GitHub permite arrastrar carpetas
   completas.
3. Clic en **Commit changes**.

## 3. Activa GitHub Pages

1. En el repositorio, ve a **Settings** → **Pages** (menú de la
   izquierda).
2. En **Source**, elige la rama `main` y la carpeta `/ (root)`.
3. Clic en **Save**.
4. En unos minutos tu página estará disponible en:
   `https://TU-USUARIO.github.io/bazar-tiburon/`

## 4. Crea tu token de administrador (Personal Access Token)

Este token es como una contraseña que le permite a la página guardar
cambios en tu repositorio. Solo tú debes tenerlo.

1. Ve a
   [github.com/settings/personal-access-tokens/new](https://github.com/settings/personal-access-tokens/new)
2. **Token name:** algo como `bazar-tiburon-admin`.
3. **Expiration:** elige 90 días o 1 año (cuando expire, simplemente
   creas uno nuevo).
4. **Repository access:** elige **Only select repositories** y
   selecciona `bazar-tiburon`.
5. **Permissions** → **Repository permissions** → busca **Contents** →
   cámbialo a **Read and write**.
6. Clic en **Generate token**.
7. Copia el token que aparece (empieza con `github_pat_...`). **Solo se
   muestra una vez** — guárdalo en un lugar seguro (por ejemplo, tu
   gestor de contraseñas).

## 5. Entra como administrador

1. Abre tu página publicada.
2. Clic en el candado 🔒 arriba a la derecha.
3. Completa:
   - **Usuario u organización de GitHub:** tu usuario (ej. `czuniga`)
   - **Nombre del repositorio:** `bazar-tiburon`
   - **Rama:** `main`
   - **Token de acceso:** pega el token del paso 4
4. Clic en **Conectar**.

Ya puedes editar: pasa el mouse sobre cualquier prenda para subir una
foto, usa el lápiz ✎ para editar nombre/precio/tallas, o "+ Agregar
prenda" / "+ Agregar categoría" para sumar más. Cada cambio se sube
solo — espera 30 segundos a 2 minutos y actualiza la página para verlo
publicado.

## Notas importantes

- **El token es privado.** Equivale a una llave de tu repositorio. No lo
  compartas ni lo pegues en mensajes públicos. Si crees que alguien más
  lo tiene, revócalo desde
  [github.com/settings/tokens](https://github.com/settings/tokens) y
  genera uno nuevo.
- El token se guarda **solo en el navegador donde inicias sesión como
  administrador**, y se borra al cerrar la pestaña — la próxima vez que
  quieras editar, tendrás que pegarlo de nuevo (o guardarlo tú mismo en
  tu gestor de contraseñas para copiarlo rápido).
- El público que visite la página **nunca ve el modo administrador ni
  necesita ningún dato de GitHub** — solo ve el catálogo.
- Usa el botón "⬇ Respaldo" en modo administrador cuando quieras
  descargar una copia del catálogo actual en tu computadora, por si
  acaso.
- Borrar una foto desde la página la desvincula de la prenda, pero no
  borra el archivo del repositorio (queda en `data/images/`). Puedes
  borrar archivos sueltos manualmente desde GitHub si quieres liberar
  espacio.
