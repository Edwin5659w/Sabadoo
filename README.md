# Sistema de Ficheros — Biblioteca Universitaria Central

Presentación web interactiva para el proyecto final de **Sistemas Operativos**.

**Autor:** Edwin Yair Molina Cerón · ID 408873

## Ver en línea

Después del despliegue en Vercel, la URL quedará en el panel de Vercel o en la salida del comando `vercel --prod`.

## Archivos

| Archivo       | Descripción                    |
|---------------|--------------------------------|
| `index.html`  | Contenido de las 8 secciones   |
| `styles.css`  | Diseño y diagramas             |
| `app.js`      | Navegación y animaciones       |

## Subir a GitHub y desplegar en Vercel

### 1. Iniciar sesión en GitHub (solo la primera vez)

```powershell
gh auth login
```

Elige **GitHub.com** → **HTTPS** → inicia sesión en el navegador.

### 2. Crear el repositorio y subir la rama `edwin`

```powershell
cd C:\2026\Universidad\SO\Sabadoo

gh repo create sistema-ficheros-biblioteca --public --source=. --remote=origin --push
```

Si el nombre ya existe en tu cuenta, usa otro, por ejemplo:

```powershell
gh repo create biblioteca-so-edwin --public --source=. --remote=origin --push
```

### 3. Desplegar en Vercel

**Opción A — Desde la web (recomendada para exponer hoy)**

1. Entra en [vercel.com](https://vercel.com) e inicia sesión con GitHub.
2. **Add New Project** → importa el repositorio que acabas de crear.
3. Deja todo por defecto (sitio estático, sin build command).
4. **Deploy**. En 1–2 minutos tendrás una URL tipo `https://tu-proyecto.vercel.app`.

**Opción B — Desde la terminal**

```powershell
cd C:\2026\Universidad\SO\Sabadoo
npx vercel login
npx vercel --prod
```

Comparte esa URL con tu clase; todos pueden abrirla al mismo tiempo durante la exposición.

## Abrir en local

Abre `index.html` en el navegador o:

```powershell
python -m http.server 8080
```

Luego visita `http://localhost:8080`.

## Tecnologías

HTML, CSS y JavaScript vanilla — sin frameworks.
