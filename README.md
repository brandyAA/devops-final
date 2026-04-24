# 🚀 DevOps Final - CI/CD con GitHub, Docker y Render

## 📌 Descripción

Este proyecto consiste en una aplicación web desarrollada como práctica final de DevOps, implementando un flujo completo de **Integración Continua y Despliegue Continuo (CI/CD)**.

La aplicación fue contenedorizada con Docker, publicada en Docker Hub y desplegada automáticamente en producción utilizando GitHub Actions y Render.

---

## 🛠 Tecnologías utilizadas

* **HTML5**
* **CSS3**
* **JavaScript**
* GitHub
* Docker
* Docker Hub
* GitHub Actions
* Render
* **Nginx (Alpine)**

---

## 📂 Estructura del proyecto

```bash
devops-final/
│── .github/
│   └── workflows/
│       └── deploy.yml
│
│── index.html
│── style.css
│── script.js
│── Dockerfile
│── README.md
```

---

## 🐳 Docker

Se creó un contenedor utilizando Nginx para servir la aplicación web.

### Dockerfile:

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

### Build:

```bash
docker build -t devops-final .
```

### Run:

```bash
docker run -p 3000:80 devops-final
```

---

## ☁️ Docker Hub

La imagen fue publicada en Docker Hub:

```bash
docker tag devops-final TU_USUARIO/devops-final:latest
docker push TU_USUARIO/devops-final:latest
```

---

## ⚙️ CI/CD con GitHub Actions

Cada vez que se hace un **push** a la rama principal:

✔ Se clona el repositorio
✔ Se construye la imagen Docker
✔ Se sube automáticamente a Docker Hub
✔ Se despliega automáticamente en Render

Esto automatiza completamente el flujo de despliegue.

---

## 🌐 Producción

Aplicación desplegada en Render:

**URL:** *(coloca aquí tu URL de Render)*

---

## 📦 Repositorio

Repositorio público:

**GitHub:** *(coloca aquí tu URL de GitHub)*

---

## 🎯 Objetivo

Aplicar conceptos de:

* Git / GitHub
* Docker
* Docker Hub
* CI/CD
* Deploy automático
* Automatización de procesos DevOps

---

## 👨‍💻 Autor

**Brandy Alcántara**
Estudiante de Desarrollo de Software
