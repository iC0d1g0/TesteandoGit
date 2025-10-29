
````markdown
# 🧭 Guía Práctica para Aprender Git y GitHub

Bienvenido/a a esta guía práctica diseñada para **aprender y practicar Git y GitHub desde cero**, de forma estructurada y experimental.  
Este repositorio no es solo teoría: aquí podrás **probar cada comando, experimentar con errores y dominar el control de versiones** como en un entorno real.

---

## 🎯 Objetivo del Repositorio

Este proyecto tiene dos propósitos principales:

1. **Servir como guía educativa**, explicando los fundamentos de Git y GitHub de forma clara y progresiva.  
2. **Funcionar como campo de práctica**, donde puedes aplicar lo aprendido sin miedo a romper nada.

---

## 📚 Contenido

Cada sección de esta guía aborda un tema esencial del flujo de trabajo con Git y GitHub.

| Sección | Tema | Qué aprenderás |
|:--|:--|:--|
| 1️⃣ | [Configuración Inicial](#-1️⃣-configuración-inicial) | Instalar, configurar e iniciar un repositorio |
| 2️⃣ | [Flujo Básico de Trabajo](#-2️⃣-flujo-básico-de-trabajo) | Cómo versionar cambios y sincronizarlos |
| 3️⃣ | [Trabajo con Ramas](#-3️⃣-trabajo-con-ramas) | Crear y fusionar líneas de desarrollo |
| 4️⃣ | [Uso de GitHub](#-4️⃣-uso-de-github) | Colaborar, hacer Pull Requests y usar Issues |
| 5️⃣ | [Buenas Prácticas](#-5️⃣-buenas-prácticas) | Organización, convenciones y hábitos sanos |

---

## 🧩 1️⃣ Configuración Inicial

Antes de empezar, asegúrate de tener **Git instalado**.  
Puedes verificarlo con:

```bash
git --version
````

Si no lo tienes, descárgalo desde [git-scm.com](https://git-scm.com/).

### 🔧 Configura tu identidad

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@correo.com"
```

Esto asegura que cada commit quede identificado correctamente.

### 🏗️ Crea un nuevo repositorio

En tu terminal:

```bash
mkdir practica-git
cd practica-git
git init
```

¡Felicidades! Acabas de crear tu primer repositorio local.

---

## ⚙️ 2️⃣ Flujo Básico de Trabajo

### 📄 Agregar archivos

Crea un archivo de ejemplo:

```bash
echo "Mi primer archivo en Git" > ejemplo.txt
```

Luego agrégalo al área de preparación (staging):

```bash
git add ejemplo.txt
```

### 💾 Guardar cambios (commit)

```bash
git commit -m "Agrego archivo de ejemplo"
```

Cada commit representa una versión estable de tu trabajo.

### 🔁 Subir y bajar cambios

Para conectar con GitHub:

1. Crea un repositorio vacío en tu cuenta de GitHub.
2. Copia la URL (por ejemplo: `https://github.com/usuario/practica-git.git`)
3. Conéctalo:

   ```bash
   git remote add origin https://github.com/usuario/practica-git.git
   git branch -M main
   git push -u origin main
   ```

A partir de ahora podrás usar `git push` y `git pull` para sincronizar cambios.

---

## 🌿 3️⃣ Trabajo con Ramas

Las ramas permiten **experimentar sin afectar la versión principal** del proyecto.

### 🌱 Crear una nueva rama

```bash
git checkout -b nueva-rama
```

Haz cambios, guárdalos y luego vuelve a `main`:

```bash
git checkout main
```

### 🔀 Fusionar ramas

Cuando una rama está lista para integrarse:

```bash
git merge nueva-rama
```

Si hay conflictos, Git te avisará para que los resuelvas manualmente.

---

## ☁️ 4️⃣ Uso de GitHub

GitHub permite **trabajar en equipo**, **compartir proyectos** y **revisar código** de forma profesional.

### 🔁 Fork y Pull Request

1. Haz un *fork* de un repositorio ajeno (una copia en tu cuenta).
2. Realiza tus cambios en una rama.
3. Abre un **Pull Request** para proponer los cambios al repositorio original.

> 💡 Un Pull Request es una solicitud de fusión: "He hecho mejoras, ¿pueden revisarlas y fusionarlas?"

### 🐞 Issues

En GitHub puedes abrir **Issues** para:

* Reportar errores
* Proponer ideas
* Discutir mejoras

### 🧩 Projects y Wikis

Explora los tableros de proyectos y las wikis de GitHub para organizar tareas y documentación colaborativa.

---

## 🧠 5️⃣ Buenas Prácticas

✅ **Commits pequeños y descriptivos**

> Ejemplo: `git commit -m "Agrego validación de usuario en formulario"`

✅ **Evita subir archivos innecesarios**
Crea un `.gitignore` con contenido como:

```
node_modules/
.env
.DS_Store
```

✅ **Usa ramas con nombres claros**

> Ejemplo: `feature/login`, `bugfix/validacion-email`

✅ **Actualiza tu rama frecuentemente**

> `git pull origin main` antes de hacer `push` o abrir un Pull Request.

---

## 🧰 Recursos Recomendados

* 📘 [Pro Git (Libro oficial gratuito)](https://git-scm.com/book/es/v2)
* 🎓 [Documentación de GitHub](https://docs.github.com/es)
* 🧑‍💻 [Try Git – Curso interactivo](https://try.github.io)
* 🔍 [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

---

## 🧾 Licencia

Este repositorio se distribuye bajo la **Licencia MIT**, lo que permite su uso, modificación y redistribución con la debida atribución.

---

## ✍️ Autor

Creado por **[Tu Nombre o Usuario de GitHub]**
💬 Propósito: Aprender, practicar y enseñar Git & GitHub de forma clara, divertida y progresiva.

---

> “Aprender Git no se trata solo de comandos, sino de entender cómo piensan los sistemas de control de versiones. Cuanto más practiques, más natural se vuelve.”


