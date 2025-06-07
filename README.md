<div align="center">

# InstaRuta 🚌

![Next](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white&style=for-the-badge)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)

![GitHub last commit](https://img.shields.io/github/last-commit/Flying-Spaghetti-Monster69/instaruta)
![GitHub issues](https://img.shields.io/github/issues/Flying-Spaghetti-Monster69/instaruta)
![GitHub pull requests](https://img.shields.io/github/issues-pr/Flying-Spaghetti-Monster69/instaruta)
![License](https://img.shields.io/github/license/Flying-Spaghetti-Monster69/instaruta)

**InstaRuta** es una aplicación web innovadora que permite a los usuarios rastrear y monitorear rutas de transporte público en tiempo real. Esta plataforma está desarrollada con tecnologías modernas para ofrecer una experiencia fluida y eficiente a nuestros usuarios.

[🌐 Demo en Vivo](https://instaruta.vercel.app) • [📋 Reportar Bug](https://github.com/Flying-Spaghetti-Monster69/instaruta/issues) • [💡 Solicitar Feature](https://github.com/Flying-Spaghetti-Monster69/instaruta/issues)

</div>

---

## 📚 Tabla de Contenidos

- [🌟 Características](#-características)
- [🛠️ Tecnologías Utilizadas](#️-tecnologías-utilizadas)
- [📋 Requisitos Previos](#-requisitos-previos)
- [🚀 Instalación](#-instalación)
- [📱 Comandos Disponibles](#-comandos-disponibles)
- [🏗️ Estructura del Proyecto](#️-estructura-del-proyecto)
- [🎯 Uso y Desarrollo](#-uso-y-desarrollo)
- [🌐 Despliegue](#-despliegue)
- [🤝 Contribuir](#-contribuir)
- [📄 Licencia](#-licencia)
- [🆘 Soporte](#-soporte)

---

## 🌟 Características

<table>
<tr>
<td>

- ⚡ **Next.js** - Framework web moderno y rápido
- ⚛️ **React** - Componentes interactivos
- 🎨 **TailwindCSS** - Estilos modernos y responsive

</td>
<td>

- 🗺️ **Mapas en tiempo real** - Seguimiento de rutas
- 📱 **Responsive Design** - Optimizado para todos los dispositivos
- 🔥 **Fast Refresh** - Desarrollo rápido con recarga automática

</td>
</tr>
</table>

## 🛠️ Tecnologías Utilizadas

| Tecnología                                                                                                | Versión  | Propósito                 |
| --------------------------------------------------------------------------------------------------------- | -------- | ------------------------- |
| ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)         | `13.3.3` | Framework principal       |
| ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)                | `19.0.0` | Biblioteca de componentes |
| ![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat&logo=tailwind-css&logoColor=white) | `3.3.0`  | Framework de CSS          |
| ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white)  | `5.0.0`  | Tipado estático           |
| ![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat&logo=pnpm&logoColor=white)                    | `Latest` | Gestor de paquetes        |

---

## 📋 Requisitos Previos

> [!IMPORTANT]
> Antes de comenzar, asegúrate de tener instalado:

- **Node.js** (versión 18 o superior) ✅
- **pnpm** (recomendado) o npm/yarn ✅

<details>
<summary><strong>🔧 Instalar pnpm (si no lo tienes)</strong></summary>

```bash
# Usando npm
npm install -g pnpm

# Usando Homebrew (macOS)
brew install pnpm

# Usando Chocolatey (Windows)
choco install pnpm
```

</details>

---

## 🚀 Instalación

> [!TIP]
> Sigue estos pasos para configurar el proyecto localmente:

### **Método 1: Clonación tradicional**

```bash
# 1️⃣ Clona el repositorio
git clone https://github.com/Flying-Spaghetti-Monster69/instaruta.git
cd instaruta
# 2️⃣ Instala las dependencias
pnpm install

# 3️⃣ Inicia el servidor de desarrollo
pnpm dev
```

### **Método 2: Usando degit (más rápido)**

```bash
# 1️⃣ Clona sin historial de git
npx degit Flying-Spaghetti-Monster69/instaruta my-instarutacd my-instaruta
# 2️⃣ Instala las dependencias
pnpm install

# 3️⃣ Inicia el servidor de desarrollo
pnpm dev
```

### **🌐 Abre tu navegador**

Visita [http://localhost:3000](http://localhost:3000) para ver la aplicación.

> [!NOTE]
> El puerto puede cambiar automáticamente si 3000 está ocupado. Revisa la terminal para ver el puerto exacto.

---

## 📱 Comandos Disponibles

<div align="center">

| Comando      | Descripción                                | Uso              |
| ------------ | ------------------------------------------ | ---------------- |
| `pnpm dev`   | 🚀 Inicia el servidor de desarrollo        | Desarrollo local |
| `pnpm build` | 🏗️ Construye la aplicación para producción | Deploy           |
| `pnpm start` | 👀 Inicia el servidor de producción        | Testing          |
| `pnpm lint`  | ⚙️ Ejecuta el linter                       | Utilidades       |

</div>

---

## 🏗️ Estructura del Proyecto

```
instaruta/
├── app/              # Next.js app router pages
├── components/       # Reusable UI components
├── prisma/          # Database schema and migrations
├── public/          # Static assets
└── utils/           # Helper functions and constants
```

---

## 🎯 Uso y Desarrollo

<details>
<summary><strong>➕ Añadir Nuevos Componentes</strong></summary>

1. **Crea tu componente en `components/`**
2. **Importa y usa el componente en tus páginas**

```tsx
// components/MiComponente.tsx
import React from "react";

interface Props {
  title: string;
  description?: string;
}

export default function MiComponente({ title, description }: Props) {
  return (
    <div className="p-4 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg">
      <h2 className="text-white font-bold text-xl">{title}</h2>
      {description && <p className="text-blue-100 mt-2">{description}</p>}
    </div>
  );
}
```

</details>

<details>
<summary><strong>📄 Crear Nuevas Páginas</strong></summary>

1. **Añade archivos `.tsx` en `app/`**
2. **Las rutas se generan automáticamente basadas en la estructura de archivos**

```tsx
// app/about/page.tsx
import { Metadata } from "next";
import MiComponente from "@/components/MiComponente";

export const metadata: Metadata = {
  title: "Acerca de InstaRuta",
};

export default function AboutPage() {
  return (
    <main className="container mx-auto px-4 py-8">
      <h1 className="text-4xl font-bold mb-8">Acerca de InstaRuta</h1>
      <MiComponente
        title="Nuestra Misión"
        description="Facilitar el acceso al transporte público"
      />
    </main>
  );
}
```

</details>

---

## 🌐 Despliegue

<div align="center">

### 🏗️ **Build para Producción**

```bash
pnpm build
```

### 👀 **Previsualizar Build**

```bash
pnpm preview
```

</div>

> [!NOTE]
> Los archivos optimizados se generarán en el directorio `dist/`.

<details>
<summary><strong>🚀 Opciones de Despliegue</strong></summary>

| Plataforma       | Comando                         | Documentación                                                           |
| ---------------- | ------------------------------- | ----------------------------------------------------------------------- |
| **Vercel**       | `vercel --prod`                 | [Guía de Vercel](https://nextjs.org/docs/deployment#vercel)             |
| **Netlify**      | `netlify deploy --prod`         | [Guía de Netlify](https://nextjs.org/docs/deployment#netlify)           |
| **GitHub Pages** | `pnpm build && gh-pages -d out` | [Guía de GitHub Pages](https://nextjs.org/docs/deployment#github-pages) |

</details>

---

### 🚀 \*\*Cómo Hacer un Commit

<details>
<summary><strong>1️⃣ Configurar Git (primera vez)</strong></summary>

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"

# Configuración adicional recomendada
git config --global init.defaultBranch main
git config --global pull.rebase false
```

</details>

<details>
<summary><strong>2️⃣ Clonar y Configurar el Repositorio</strong></summary>

```bash
git clone https://github.com/Flying-Spaghetti-Monster69/instaruta.git
cd instarutagit checkout develop
```

</details>

<details>
<summary><strong>3️⃣ Crear una Nueva Feature</strong></summary>

```bash
# Asegúrate de estar en develop
git checkout develop
git pull origin develop

# Crear y cambiar a una nueva rama feature
git checkout -b feature/nombre-de-tu-feature

# Ejemplo:
git checkout -b feature/add-contact-form
```

</details>

<details>
<summary><strong>4️⃣ Desarrollar tu Feature</strong></summary>

```bash
# Hacer cambios en el código
# Guardar archivos

# Ver el estado de los archivos
git status

# Añadir archivos al staging area
git add .
# O añadir archivos específicos:
git add components/ContactForm.tsx

# Hacer commit con mensaje descriptivo
git commit -m "feat: añadir formulario de contacto con validación"
```

</details>

<details>
<summary><strong>5️⃣ Convenciones para Mensajes de Commit</strong></summary>

> [!TIP]
> Usa estos prefijos para mantener consistencia:

| Prefijo     | Descripción                  | Ejemplo                                            |
| ----------- | ---------------------------- | -------------------------------------------------- |
| `feat:`     | ✨ Nueva funcionalidad       | `feat: añadir componente de navegación responsiva` |
| `fix:`      | 🐛 Corrección de bug         | `fix: corregir problema de scroll en mobile`       |
| `docs:`     | 📚 Cambios en documentación  | `docs: actualizar README con instrucciones`        |
| `style:`    | 💄 Cambios de formato        | `style: mejorar espaciado en componente Hero`      |
| `refactor:` | ♻️ Refactorización de código | `refactor: optimizar componente ShinyText`         |
| `test:`     | ✅ Añadir o modificar tests  | `test: añadir tests para ContactForm`              |
| `chore:`    | 🔧 Tareas de mantenimiento   | `chore: actualizar dependencias`                   |

</details>

<details>
<summary><strong>6️⃣ Subir tu Feature</strong></summary>

```bash
# Subir tu rama al repositorio remoto
git push origin feature/nombre-de-tu-feature

# Ejemplo:
git push origin feature/add-contact-form
```

</details>

<details>
<summary><strong>7️⃣ Crear Pull Request</strong></summary>

1. **Ve a GitHub** 🌐
2. **Haz clic en "Compare & pull request"** 🔄
3. **Describe tu cambio** 📝
4. **Asigna reviewers** 👥
5. **Espera la revisión y aprobación** ✅

> [!NOTE]
> Asegúrate de que tu PR tenga:
>
> - [ ] Título descriptivo
> - [ ] Descripción detallada de los cambios
> - [ ] Screenshots si hay cambios visuales
> - [ ] Tests pasando ✅

</details>

<details>
<summary><strong>8️⃣ Después del Merge</strong></summary>

```bash
# Volver a develop
git checkout develop

# Actualizar develop
git pull origin develop

# Eliminar la rama feature local
git branch -d feature/nombre-de-tu-feature

# Eliminar la rama feature remota (opcional)
git push origin --delete feature/nombre-de-tu-feature
```

</details>

---

### 🚨 **Hotfixes Urgentes**

> [!CAUTION]
> Solo para correcciones críticas en producción:

```bash
# Crear hotfix desde main
git checkout main
git pull origin main
git checkout -b hotfix/descripcion-del-fix

# Hacer cambios y commit
git add .
git commit -m "hotfix: corregir error crítico en formulario"

# Subir hotfix
git push origin hotfix/descripcion-del-fix

# Crear PR hacia main Y develop
```

---

### 📝 **Comandos Útiles de Git**

<details>
<summary><strong>🔍 Ver y Explorar</strong></summary>

```bash
# Ver historial de commits
git log --oneline --graph --all

# Ver diferencias antes de commit
git diff

# Ver archivos modificados
git status -s

# Ver información de una rama
git show-branch
```

</details>

<details>
<summary><strong>↩️ Deshacer Cambios</strong></summary>

```bash
# Deshacer cambios no guardados en un archivo
git checkout -- archivo.js

# Deshacer último commit (mantener cambios)
git reset --soft HEAD~1

# Deshacer último commit (eliminar cambios)
git reset --hard HEAD~1

# Deshacer cambios en staging area
git reset HEAD archivo.js
```

</details>

<details>
<summary><strong>🌿 Gestión de Ramas</strong></summary>

```bash
# Ver ramas locales
git branch

# Ver ramas remotas
git branch -r

# Ver todas las ramas
git branch -a

# Eliminar rama local
git branch -d nombre-rama

# Eliminar rama remota
git push origin --delete nombre-rama

# Actualizar lista de ramas remotas
git fetch origin --prune
```

</details>

---

## 🤝 Contribuir

¡Nos encanta recibir contribuciones! Sigue estos pasos:

1. **🍴 Fork el proyecto**
2. **🌿 Crea una rama feature** (`git checkout -b feature/AmazingFeature`)
3. **💾 Commit tus cambios** (`git commit -m 'feat: add some AmazingFeature'`)
4. **📤 Push a la rama** (`git push origin feature/AmazingFeature`)
5. **🔄 Abre un Pull Request**

### 📋 **Checklist para Contributors**

- [ ] He leído la guía de contribución
- [ ] Mi código sigue las convenciones del proyecto
- [ ] He añadido tests para mi funcionalidad
- [ ] Todos los tests existentes pasan
- [ ] He actualizado la documentación si es necesario
- [ ] Mi commit sigue las convenciones de mensajes

---

## 📄 Licencia

Este proyecto está bajo la **Licencia MIT**. Ver el archivo [`LICENSE`](./LICENSE) para más detalles.

```
MIT License - see the [LICENSE](./LICENSE) file for details
```

---

## 🆘 Soporte

<div align="center">

### 💬 **¿Necesitas Ayuda?**

| Canal                   | Enlace                                                                                    | Propósito          |
| ----------------------- | ----------------------------------------------------------------------------------------- | ------------------ |
| 📧 **Email**            | [fgarzonm@unal.edu.co](mailto:fgarzonm@unal.edu.co)                                       | Soporte general    |
| 🐛 **Bug Reports**      | [GitHub Issues](https://github.com/Flying-Spaghetti-Monster69/instaruta/issues)           | Reportar problemas |
| 💡 **Feature Requests** | [GitHub Discussions](https://github.com/Flying-Spaghetti-Monster69/instaruta/discussions) | Nuevas ideas       |

</div>

> [!NOTE]
> Para reportes de bugs, por favor incluye:
>
> - Versión del navegador
> - Pasos para reproducir el problema
> - Screenshots si es posible
> - Logs de la consola

---

<div align="center">

### 🌟 **¡Dale una estrella si te gusta el proyecto!**

[![GitHub stars](https://img.shields.io/github/stars/Flying-Spaghetti-Monster69/instaruta?style=social)](https://github.com/Flying-Spaghetti-Monster69/instaruta/stargazers)

**Desarrollado con ❤️ por el equipo de InstaRuta**

[⬆️ Volver al inicio](#-InstaRuta)

</div>
