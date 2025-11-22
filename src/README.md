# 🎓 FISC - Ingeniería de Sistemas y Computación

Plataforma web interactiva para estudiantes de Ingeniería de Sistemas. Explora el roadmap académico completo, compara áreas electivas y descubre tu especialización ideal mediante un quiz vocacional.

---

## 🌟 Características

- ✅ **Roadmap Interactivo**: Visualiza los 46 cursos organizados por semestres con códigos, créditos y prerrequisitos
- ✅ **Comparación de Áreas**: Explora 3 rutas de especialización (Redes/Cloud, Desarrollo de Software, Desarrollo Web)
- ✅ **Quiz Vocacional**: 20 preguntas inteligentes con sistema de puntuación balanceado
- ✅ **Resultados Personalizados**: Recomendaciones basadas en tus respuestas
- ✅ **Diseño Moderno**: UI futurista con colores tech y microinteracciones suaves
- ✅ **100% Responsive**: Funciona perfectamente en móvil, tablet y desktop

---

## 🚀 Quick Start

### Desarrollo Local

```bash
# 1. Instalar dependencias
npm install

# 2. Iniciar servidor de desarrollo
npm run dev
```

Abre [http://localhost:5173](http://localhost:5173) en tu navegador.

### Build para Producción

```bash
# Compilar proyecto
npm run build

# Vista previa del build
npm run preview
```

---

## 📦 Deploy a GitHub Pages

### Método 1: Script Automático (Recomendado)

**Windows:**
```bash
deploy.bat
```

**Linux/Mac:**
```bash
chmod +x deploy.sh
./deploy.sh
```

### Método 2: Manual

```bash
# 1. Build del proyecto
npm run build

# 2. Verificar que se creó la carpeta docs/
# La carpeta docs/ se genera automáticamente desde dist/

# 3. Subir a GitHub
git add .
git commit -m "Deploy: FISC Platform"
git push origin main

# 4. Configurar GitHub Pages
# Ve a: Settings → Pages
# Source: main
# Folder: /docs
# Save
```

### Configuración de GitHub Pages

1. Ve a tu repositorio en GitHub
2. **Settings** → **Pages**
3. Selecciona:
   - **Source**: `main`
   - **Folder**: `/docs`
4. Click **Save**
5. ¡Listo! Tu sitio estará en: `https://TU_USUARIO.github.io/FISC/`

📖 **Guía Detallada**: Ver [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md)

---

## 🛠️ Tecnologías

- **React 18** - UI Library
- **TypeScript** - Type Safety
- **Vite** - Build Tool & Dev Server
- **TailwindCSS 4.0** - Styling
- **Lucide React** - Iconos
- **Poppins Font** - Tipografía

---

## 📁 Estructura del Proyecto

```
/
├── components/           # Componentes React
│   ├── Home.tsx         # Página principal
│   ├── Roadmap.tsx      # Roadmap de cursos
│   ├── TracksComparison.tsx  # Comparación de áreas
│   ├── Quiz.tsx         # Quiz vocacional
│   ├── TrackResult.tsx  # Resultados personalizados
│   ├── layout/          # Componentes de layout
│   └── quiz/            # Componentes del quiz
├── data/                # Datos estáticos
│   └── quiz-questions.ts
├── constants/           # Constantes y configuración
├── hooks/               # Custom React Hooks
├── types/               # TypeScript Types
├── styles/              # Estilos globales
│   └── globals.css
├── App.tsx              # Componente raíz
├── src/
│   └── main.tsx         # Entry point
├── index.html           # HTML principal
├── vite.config.ts       # Configuración de Vite
├── package.json         # Dependencias
├── tsconfig.json        # TypeScript config
└── deploy.sh/.bat       # Scripts de deployment
```

---

## 🎨 Paleta de Colores

```css
/* Colores principales */
--primary-blue: #4A6DFF;
--primary-purple: #7A5BFF;
--accent-mint: #56F0C3;

/* Backgrounds */
--bg-dark: #1B1E28;
--bg-medium: #252935;
```

---

## 📝 Scripts Disponibles

| Comando | Descripción |
|---------|-------------|
| `npm run dev` | Inicia servidor de desarrollo en modo hot-reload |
| `npm run build` | Compila el proyecto y genera carpeta docs/ |
| `npm run preview` | Vista previa del build de producción |

---

## 🔧 Configuración para GitHub Pages

El proyecto ya está configurado para GitHub Pages con:

- ✅ `base: '/FISC/'` en `vite.config.ts`
- ✅ Build automático que genera carpeta `docs/`
- ✅ Rutas relativas para assets
- ✅ Scripts de deployment automatizados

---

## 📚 Contenido Académico

### Roadmap Completo
- **46 cursos** organizados en 10 semestres
- Información detallada: código, nombre, créditos, tipo, prerrequisitos
- Total: 200+ créditos

### Áreas Electivas (7º Semestre)

1. **🌐 Redes, Servidores y Cloud**
   - Infraestructura tecnológica
   - Administración de servidores
   - Cloud computing

2. **💻 Desarrollo de Software**
   - Arquitecturas empresariales
   - Patrones de diseño
   - Metodologías ágiles

3. **🚀 Desarrollo Web**
   - Frontend moderno
   - Backend escalable
   - Full stack development

### Quiz Vocacional
- 20 preguntas estratégicas
- 4 bloques temáticos
- Sistema de puntuación balanceado
- Resultados personalizados

---

## 🐛 Troubleshooting

### El sitio no carga en GitHub Pages

**Solución:**
- Verifica que la carpeta sea `/docs` en GitHub Pages
- Confirma que `vite.config.ts` tenga `base: '/FISC/'`

### Errores en npm run build

**Solución:**
```bash
rm -rf node_modules package-lock.json
npm install
npm run build
```

### Las imágenes no cargan

**Solución:**
- Las imágenes de Figma se importan automáticamente
- Vite maneja las rutas con el `base` configurado

---

## 📄 Licencia

Este proyecto es de código abierto y está disponible para uso educativo.

---

## 👥 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

---

## 📧 Contacto

**Proyecto FISC** - Ingeniería de Sistemas y Computación

---

## 🎯 Roadmap del Proyecto

- [x] Diseño UI/UX completo
- [x] Implementación del Roadmap
- [x] Sistema de Quiz vocacional
- [x] Comparación de áreas electivas
- [x] Resultados personalizados
- [x] Configuración para GitHub Pages
- [ ] Sistema de recursos adicionales
- [ ] Integración con APIs académicas
- [ ] Dashboard de seguimiento académico

---

## ⭐ ¿Te gustó el proyecto?

Si este proyecto te ayudó, considera darle una ⭐ en GitHub.

---

**Desarrollado con ❤️ para estudiantes de Ingeniería de Sistemas**

© 2025 PJ - Todos los derechos reservados
