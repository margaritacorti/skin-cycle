# SkinCycle 🌸

Una app web minimalista para personalizar y trackear tu rutina de skincare con ciclos de 3 días.

## 📱 Características

✨ **Rutina personalizada** - Crea tu propio ciclo de 3 días con pasos AM y PM  
📅 **Tracker visual** - Calendario para marcar días completados y ver rachas  
💭 **Chat con IA** - Habla con Claude para recomendaciones de productos  
📊 **Dashboard intuitivo** - Tres vistas: hoy, tracker, rutina completa  
🎨 **Diseño glassmorphism** - Interfaz translúcida moderna  
📱 **iPhone 14 optimizado** - Responsive y touch-friendly  

---

## 🚀 Instalación Rápida

### Opción 1: Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/skincycle.git
cd skincycle
```

Luego abre `index.html` en tu navegador.

### Opción 2: Usar directamente (GitHub Pages)

Si está deployado en GitHub Pages:
```
https://tu-usuario.github.io/skincycle
```

### Opción 3: Descargar ZIP

1. Click en **Code** → **Download ZIP**
2. Descomprime
3. Abre `index.html`

---

## 📖 Guía de Uso

### 1️⃣ Crear tu rutina (`index.html`)

```
Tu Rutina → personaliza tus pasos diarios

Básico:
  • Nombre: "tu nombre"
  • Tipo de piel: Seca / Grasa / Mixta / Sensible

Día 1, Día 2, Día 3:
  • AM: agrega pasos
  • PM: agrega pasos
  
[limpiar todo] [guardar rutina]
```

### 2️⃣ Dashboard principal (`main.html`)

**Tab: Hoy**
- AM/PM con pasos actuales
- Botón "marcar como completada"
- Botón "💬 hablar con IA"

**Tab: Tracker**
- Calendario últimos 7 días
- Días completados en verde
- Stats: días completados + racha actual

**Tab: Rutina**
- Vista de los 3 días completos
- Perfil (nombre, tipo de piel)
- Botón "editar rutina"

---

## 🛠️ Tecnología

- **HTML5** - Estructura semántica
- **CSS3** - Glassmorphism, gradientes, transiciones
- **JavaScript Vanilla** - Sin frameworks, localStorage para datos
- **Responsive** - Optimizado para iPhone 14 (375px)

---

## 📁 Estructura de archivos

```
skincycle/
├── index.html          # Crear/editar rutina
├── main.html           # Dashboard principal
├── README.md           # Este archivo
├── .gitignore          # Archivos ignorados
└── LICENSE             # MIT License
```

---

## 💾 Datos guardados (localStorage)

```javascript
{
  // Tu perfil y rutina
  skinCycleRoutine: {
    name: "tu nombre",
    skinType: "Sensible",
    days: {
      day1: { AM: ["paso 1", "paso 2"], PM: ["paso 1"] },
      day2: { AM: [...], PM: [...] },
      day3: { AM: [...], PM: [...] }
    }
  },
  
  // Días completados
  skinCycleCompleted: {
    "2024-06-17": true,
    "2024-06-16": true,
    ...
  }
}
```

Los datos se guardan **en tu navegador**. No se envía información a servidores.

---

## 🔗 Próximas características

- [ ] Conectar Claude API para chat IA con recomendaciones
- [ ] Notificaciones push (PWA)
- [ ] Exportar rutina (PDF/email)
- [ ] Multi-idioma (EN, ES, PT)
- [ ] Modo oscuro/claro
- [ ] Sincronización cloud

---

## 🤝 Contribuir

¿Encontraste un bug o tienes una idea? ¡Abre un [issue](https://github.com/tu-usuario/skincycle/issues)!

---

## 📄 Licencia

MIT License - Libre para usar, modificar y distribuir.

---

## 👤 Autor

Hecho con 💜 para skincare lovers.

---

**¿Preguntas?** Abre un issue en GitHub o contacta directamente.
