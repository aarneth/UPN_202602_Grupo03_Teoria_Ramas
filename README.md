# ☕ Java & Git Learning Lab

Repositorio colaborativo de aprendizaje práctico enfocado en el desarrollo en **Java** y el dominio del control de versiones con **Git** y **GitHub**, elaborado por estudiantes de la **Universidad Privada del Norte (UPN)**.

---

## 📌 Descripción del Proyecto

Este espacio académico tiene como propósito consolidar las bases del flujo de trabajo profesional con Git y GitHub aplicados al ecosistema Java. A lo largo del proyecto se implementan prácticas de gestión de ramas (*branches*), resolución de conflictos, sincronización remota e integración de código colaborativo.

---

## 👥 Integrantes del Equipo

* **Graciela Ruiz Ramos**
* **Alejandro Huilcaya**
* **Aaron Gonzales Cortez**

> **Institución:** Universidad Privada del Norte (UPN)

---

## 🛠️ Tecnologías y Entornos

* **Lenguaje:** Java (JDK 17+)
* **Control de Versiones:** Git
* **Alojamiento Remoto:** GitHub
* **IDE Recomendado:** IntelliJ IDEA / Eclipse / VS Code

---

## 🚀 Hoja de Ruta de Comandos Git

En este repositorio practicamos y documentamos los comandos clave de la consola:

### 1. Inicialización y Conexión Remota
```bash
# Inicializar repositorio local
git init

# Vincular con GitHub
git remote add origin https://github.com/<usuario>/<repositorio>.git

# Verificar remotos vinculados
git remote -v
```

### 2. Ciclo de Trabajo Básico (Staging y Commit)
```bash
# Comprobar estado de archivos
git status

# Agregar todos los cambios al staging area
git add .

# Guardar los cambios con un mensaje claro
git commit -m "feat: estructura base del proyecto java"
```

### 3. Sincronización Remota
```bash
# Subir la rama local por primera vez
git push -u origin main

# Descargar e integrar cambios remotos
git pull origin main
```

### 4. Gestión de Ramas (*Branching*)
```bash
# Listar ramas locales
git branch

# Crear y moverse a una nueva rama de trabajo
git checkout -b feature/logica-java
# Alternativa moderna:
git switch -c feature/logica-java

# Cambiar de rama
git checkout main
# o:
git switch main

# Integrar cambios de una rama secundaria
git merge feature/logica-java

# Publicar la rama en el repositorio remoto
git push -u origin feature/logica-java
```

---

## 📂 Estructura Base Sugerida

```text
├── src/                  # Clases y ejercicios en Java
│   └── Main.java
├── .gitignore            # Archivos excluidos (.class, /bin, .idea, etc.)
└── README.md             # Documentación principal
```

---

## 🤝 Buenas Prácticas del Equipo

1. **Trabajo en ramas:** Trabajar siempre en ramas dedicadas (`feature/`, `fix/`) antes de integrar a `main`.
2. **Mensajes claros:** Usar mensajes de confirmación descriptivos y directos.
3. **Pull antes de Push:** Mantener el repositorio local siempre actualizado antes de subir cambios.