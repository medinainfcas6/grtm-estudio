# Bitácora GRTM

Web de estudio de **Gestión y Regulación del Transporte Marítimo** (4º GTL, UPV): apuntes de cada tema, mapa mental, banco de preguntas del profesor resuelto, preguntas extra y un examen personalizado de respuesta corta que corrige Claude.

Es una sola página (`index.html`), sin compilar nada.

## Publicarla con GitHub Pages

1. Sube `index.html`, `.nojekyll` y este `README.md` a la raíz del repositorio (rama `main`).
2. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`, **Save**.
3. Al cabo de uno o dos minutos la web queda en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Corrección con IA

GitHub Pages solo sirve archivos estáticos, así que la corrección del examen llama a la API de Claude directamente desde el navegador:

- En **Examen personalizado → Corrección con IA** se pega una clave de API de Claude (`sk-ant-…`, se crea en platform.claude.com).
- La clave se guarda **solo en el `localStorage` de ese navegador**. No está en el repositorio ni se envía a ningún sitio salvo a `api.anthropic.com`.
- **No subas nunca la clave al repositorio.** Si la web es pública, quien la abra tendrá que poner su propia clave.
- Sin clave se puede hacer el examen igual y compararlo con las respuestas modelo.

Las marcas «La sé / Repasar», el historial de exámenes y las respuestas a medias también se guardan solo en el navegador.
