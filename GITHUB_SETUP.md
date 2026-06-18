# Guía: Crear repositorio en GitHub

## 📋 Pasos para subir SkinCycle a GitHub

### 1️⃣ Crear repositorio en GitHub

1. Ve a [github.com/new](https://github.com/new)
2. **Repository name**: `skincycle`
3. **Description**: `App web para personalizar y trackear rutina de skincare`
4. **Public** (para que todos puedan usar)
5. Click **Create repository**

---

### 2️⃣ Configurar Git en tu computadora

```bash
# Abre Terminal/CMD en la carpeta del proyecto

# Inicializar repositorio
git init

# Agregar todos los archivos
git add .

# Primer commit
git commit -m "Initial commit: SkinCycle app"

# Agregar el repositorio remoto (reemplaza TU_USUARIO)
git remote add origin https://github.com/TU_USUARIO/skincycle.git

# Subir a GitHub
git push -u origin main
```

> **Nota:** Si tienes error "main", usa `git branch -M main` antes de push

---

### 3️⃣ Archivos incluidos

```
✓ index.html       → Crear rutina
✓ main.html        → Dashboard principal
✓ README.md        → Documentación
✓ package.json     → Metadata
✓ .gitignore       → Archivos ignorados
```

---

## 🚀 Deploy en GitHub Pages

### Opción A: Automático (Recomendado)

1. Ve a **Settings** del repo
2. Scroll a **Pages**
3. **Source**: Branch `main`, folder `/root`
4. Click **Save**
5. Espera 1 min
6. Tu app estará en: `https://TU_USUARIO.github.io/skincycle`

### Opción B: Manual con rama `gh-pages`

```bash
git checkout -b gh-pages
git push -u origin gh-pages
```

Luego en Settings → Pages → Source → `gh-pages` branch

---

## 📝 Actualizar el repo (después de hacer cambios)

```bash
# Ver cambios
git status

# Agregar cambios
git add .

# Commit
git commit -m "Descripción de cambios"

# Subir a GitHub
git push origin main
```

---

## 🔄 Clonar el proyecto (para otros)

```bash
git clone https://github.com/TU_USUARIO/skincycle.git
cd skincycle
```

Luego abre `index.html` en el navegador.

---

## 💡 Comandos útiles

```bash
# Ver historial de commits
git log

# Ver rama actual
git branch

# Crear rama nueva
git checkout -b feature/nombre

# Volver a main
git checkout main

# Ver archivos no staged
git diff
```

---

## ⚡ Quick Setup (copia y pega)

```bash
# Paso 1: Inicializar
git init
git add .
git commit -m "Initial commit: SkinCycle app"

# Paso 2: Conectar con GitHub (reemplaza TU_USUARIO)
git branch -M main
git remote add origin https://github.com/TU_USUARIO/skincycle.git
git push -u origin main

# ¡Listo! Tu repo está en GitHub 🎉
```

---

## 📱 Compartir la app

Después de setup en GitHub Pages, comparte este link:
```
https://TU_USUARIO.github.io/skincycle
```

O el repositorio:
```
https://github.com/TU_USUARIO/skincycle
```

---

## 🆘 Troubleshooting

**Error: "Permission denied (publickey)"**
→ Configura SSH keys: [github.com/settings/keys](https://github.com/settings/keys)

**Error: "failed to push some refs"**
→ Haz `git pull origin main` primero

**¿Cómo editar README.md?**
→ Abre el archivo en GitHub → Botón ✏️ (Edit) → Commit changes

---

**¿Dudas?** Abre un issue en tu repo o ve la [guía oficial de GitHub](https://docs.github.com/en/get-started/quickstart)
