# Plan para crear PCbre desde cero 🖥️

## Objetivo Principal
Crear un sitio web educativo moderno y completo para enseñar a principiantes cómo armar una PC desde cero, con mejor diseño, estructura y contenido que la versión actual.

## Fases del Proyecto

### 📋 FASE 1: Planificación y Diseño
- [ ] **Investigación y benchmarking**
  - [ ] Analizar PCPartPicker (funcionalidades y UX) - *Estudiar cómo funciona su configurador y filtros*
  - [ ] Estudiar Tom's Hardware (contenido educativo) - *Revisar estructura de artículos y guías*
  - [ ] Revisar Newegg PC Builder (configurador) - *Analizar flujo de selección de componentes*
  - [ ] Analizar iFixit (guías paso a paso) - *Ver cómo presentan tutoriales visuales*
  - [ ] Identificar gaps en el mercado - *Qué falta en sitios existentes para principiantes*
  - [ ] Definir propuesta de valor única - *Qué hará especial a nuestro sitio*
  - [ ] Crear documento de research findings - *Resumir hallazgos en 2-3 páginas*

- [ ] **Arquitectura de información**
  - [ ] Crear user personas (principiante, intermedio) - *Definir edad, experiencia, objetivos de cada tipo de usuario*
  - [ ] Mapear customer journey completo - *Desde llegada al sitio hasta armado exitoso*
  - [ ] Definir información architecture - *Organizar contenido en categorías lógicas*
  - [ ] Crear sitemap detallado - *Mapa visual de todas las páginas y secciones*
  - [ ] Diseñar flujo de navegación principal - *Cómo usuarios navegarán entre secciones*
  - [ ] Planificar estructura de URLs - */componentes/cpu, /guias/armado, etc.*
  - [ ] Crear wireframes low-fidelity - *Bocetos simples de layout de páginas clave*
  - [ ] Validar wireframes con usuarios - *Mostrar a 3-5 personas y recoger feedback*

- [ ] **Diseño visual**
  - [ ] Definir brand identity y personalidad - *Moderno, accesible, confiable, educativo*
  - [ ] Crear paleta de colores (primarios/secundarios) - *3-4 colores principales + variaciones*
  - [ ] Seleccionar tipografías (headings/body) - *Fuentes legibles para web, máx 2 familias*
  - [ ] Diseñar sistema de iconografía - *Iconos consistentes para componentes PC*
  - [ ] Crear design system/style guide - *Documento con reglas de diseño*
  - [ ] Diseñar componentes base (buttons, cards, etc.) - *Elementos reutilizables del UI*
  - [ ] Crear mockups desktop de páginas clave - *Diseños finales de 5-6 páginas principales*
  - [ ] Crear mockups mobile responsive - *Adaptación para teléfonos y tablets*
  - [ ] Diseñar estados de interacción - *Hover, focus, loading, error states*
  - [ ] Crear prototipos interactivos - *Figma/Adobe XD con navegación funcional*

### 🛠️ FASE 2: Desarrollo Frontend
- [ ] **Setup del proyecto**
  - [ ] Crear repositorio Git con estructura inicial - *GitHub repo + .gitignore + README inicial*
  - [ ] Configurar Vite + React/Vue (decisión final) - *npm create vite@latest pcbre-v2*
  - [ ] Setup Tailwind CSS + configuración custom - *Instalar + configurar colores personalizados*
  - [ ] Configurar ESLint + Prettier - *Reglas de código consistente y formato automático*
  - [ ] Setup TypeScript (opcional) - *Para mejor desarrollo y menos errores*
  - [ ] Configurar Husky para pre-commit hooks - *Validar código antes de cada commit*
  - [ ] Setup environment variables - *Archivo .env para configuraciones*
  - [ ] Configurar hot reload y dev server - *Recarga automática durante desarrollo*
  - [ ] Crear scripts de build y deploy - *npm run build, npm run preview*

- [ ] **Sistema de componentes base**
  - [ ] Crear Button component (variants, sizes) - *Primary, secondary, outline + sm/md/lg*
  - [ ] Crear Card component (diferentes tipos) - *Para componentes PC, guías, productos*
  - [ ] Crear Input/Form components - *Text, select, checkbox, radio con validación*
  - [ ] Crear Modal/Dialog component - *Para detalles de componentes y confirmaciones*
  - [ ] Crear Loading/Spinner components - *Estados de carga para herramientas*
  - [ ] Crear Toast/Notification system - *Mensajes de éxito, error, info*
  - [ ] Crear Tooltip component - *Explicaciones rápidas de términos técnicos*
  - [ ] Crear Breadcrumb component - *Navegación de ubicación actual*
  - [ ] Crear Progress bar component - *Para tutorial de armado paso a paso*
  - [ ] Documentar componentes (Storybook?) - *Guía de uso de cada componente*

- [ ] **Layout y navegación**
  - [ ] Crear Header component responsivo - *Logo + menú principal + CTA button*
  - [ ] Implementar menú hamburguesa mobile - *Navegación colapsible para móviles*
  - [ ] Crear Footer con links útiles - *Contacto, redes sociales, mapa del sitio*
  - [ ] Implementar sidebar navigation (si aplica) - *Para sección de guías detalladas*
  - [ ] Crear layout wrapper principal - *Container con padding y max-width*
  - [ ] Implementar sticky navigation - *Header fijo al hacer scroll*
  - [ ] Agregar breadcrumbs navigation - *Mostrar ubicación en jerarquía*
  - [ ] Crear skip links para accesibilidad - *Saltar al contenido principal*

- [ ] **Páginas principales - Estructura**
  - [ ] Landing page - Hero section - *Título impactante + imagen + CTA principal*
  - [ ] Landing page - Features overview - *3-4 características clave del sitio*
  - [ ] Landing page - Call to action - *Botón "Empezar a armar mi PC"*
  - [ ] Página Componentes - Lista categorizada - *CPU, GPU, RAM, etc. con imágenes*
  - [ ] Página Componentes - Filtros y búsqueda - *Por precio, marca, compatibilidad*
  - [ ] Página Componentes - Vista detalle - *Specs, compatibilidad, precios*
  - [ ] Página Compatibilidad - Checker tool - *Formulario para verificar componentes*
  - [ ] Página Armado - Steps navigation - *Menú lateral con pasos 1-10*
  - [ ] Página Armado - Progress tracking - *Barra de progreso visual*
  - [ ] Página Periféricos - Grid layout - *Monitor, teclado, mouse en grilla*

### 📝 FASE 3: Contenido y Funcionalidades
- [ ] **Contenido educativo detallado**
  - [ ] Escribir guía "Qué es cada componente" - *Explicación simple de CPU, GPU, RAM, etc.*
  - [ ] Crear guía "Cómo elegir CPU" - *Intel vs AMD, cores, frecuencia, uso*
  - [ ] Crear guía "Cómo elegir GPU" - *Gaming vs trabajo, VRAM, marcas*
  - [ ] Crear guía "RAM: tipos y capacidades" - *DDR4 vs DDR5, 16GB vs 32GB*
  - [ ] Crear guía "Motherboards y compatibilidad" - *Sockets, chipsets, features*
  - [ ] Crear guía "Fuentes de poder (PSU)" - *Wattage, eficiencia, modular vs no*
  - [ ] Crear guía "Almacenamiento: SSD vs HDD" - *Velocidad, capacidad, precios*
  - [ ] Crear guía "Cooling: aire vs líquido" - *Temperaturas, ruido, instalación*
  - [ ] Crear guía "Cases: tamaños y features" - *ATX, mATX, ITX, airflow*
  - [ ] Escribir glosario de términos (A-Z) - *TDP, PCIe, BIOS, etc. explicados*
  - [ ] Crear FAQ con 20+ preguntas comunes - *"Cuánto cuesta?", "Es difícil?", etc.*
  - [ ] Optimizar imágenes para web - *Comprimir, WebP, lazy loading*
  - [ ] Crear diagramas explicativos - *Flujo de datos, conexiones, layouts*

- [ ] **Herramientas interactivas**
  - [ ] Calculadora de compatibilidad CPU-Motherboard - *Verificar socket, chipset, BIOS*
  - [ ] Calculadora de PSU (wattage necesario) - *Sumar consumo de todos los componentes*
  - [ ] Configurador por presupuesto ($500-$3000) - *Sugerir builds por rango de precio*
  - [ ] Comparador de componentes (lado a lado) - *Specs, precios, pros/cons*
  - [ ] Checklist interactivo de armado - *Marcar pasos completados*
  - [ ] Estimador de performance (gaming/trabajo) - *FPS esperados, benchmarks*
  - [ ] Generador de lista de compras - *Export a PDF/Excel con links*
  - [ ] Calculadora de bottleneck - *Identificar cuellos de botella*

- [ ] **Funcionalidades avanzadas**
  - [ ] Implementar búsqueda con filtros - *Por precio, marca, tipo, compatibilidad*
  - [ ] Sistema de favoritos (localStorage) - *Guardar componentes preferidos*
  - [ ] Configuraciones guardadas - *Builds completos en localStorage*
  - [ ] Toggle modo oscuro/claro - *Preferencia del usuario persistente*
  - [ ] Compartir configuraciones (URL) - *Links únicos para cada build*
  - [ ] Print-friendly pages - *CSS optimizado para impresión*
  - [ ] Accesibilidad: alt texts - *Descripciones de todas las imágenes*
  - [ ] Accesibilidad: keyboard navigation - *Tab, Enter, flechas funcionan*
  - [ ] Accesibilidad: screen reader support - *ARIA labels y roles*
  - [ ] Accesibilidad: color contrast - *Cumplir WCAG 2.1 AA*

- [ ] **Contenido multimedia**
  - [ ] Grabar video "Primer armado paso a paso" - *15-20 min, calidad 1080p*
  - [ ] Crear video "Instalación de CPU" - *Close-up, 3-5 minutos*
  - [ ] Crear video "Instalación de RAM" - *Mostrar orientación correcta*
  - [ ] Crear video "Conexión de cables" - *PSU, SATA, front panel*
  - [ ] Optimizar videos para web - *Compresión, múltiples resoluciones*
  - [ ] Agregar subtítulos a videos - *Español e inglés*
  - [ ] Crear galería de imágenes por paso - *Fotos HD de cada proceso*

### 🚀 FASE 4: Optimización y Lanzamiento
- [ ] **Performance y SEO**
  - [ ] Optimizar imágenes (WebP, lazy loading) - *Compresión automática, carga bajo demanda*
  - [ ] Implementar code splitting por rutas - *Cargar solo JS necesario por página*
  - [ ] Minificar CSS y JavaScript - *Reducir tamaño de archivos*
  - [ ] Configurar caching estratégico - *Headers de cache, service worker*
  - [ ] Optimizar Core Web Vitals (LCP, FID, CLS) - *Métricas de Google PageSpeed*
  - [ ] Crear sitemap.xml - *Mapa del sitio para buscadores*
  - [ ] Configurar meta tags por página - *Title, description, keywords*
  - [ ] Implementar structured data (JSON-LD) - *Rich snippets para Google*
  - [ ] Configurar Open Graph tags - *Preview en redes sociales*
  - [ ] Setup robots.txt - *Qué pueden indexar los bots*
  - [ ] Implementar canonical URLs - *Evitar contenido duplicado*

- [ ] **Testing exhaustivo**
  - [ ] Testing en Chrome, Firefox, Safari, Edge - *Compatibilidad cross-browser*
  - [ ] Testing responsive (mobile, tablet, desktop) - *Breakpoints 320px, 768px, 1024px+*
  - [ ] Testing en dispositivos reales - *iPhone, Android, iPad físicos*
  - [ ] Validación HTML/CSS - *W3C validator, sin errores*
  - [ ] Testing de accesibilidad (WAVE, axe) - *Herramientas automáticas*
  - [ ] Performance testing (Lighthouse) - *Score 90+ en todas las métricas*
  - [ ] Testing de formularios - *Validación, envío, errores*
  - [ ] Testing de herramientas interactivas - *Calculadoras, configurador*
  - [ ] User testing con 5+ usuarios reales - *Observar uso real*
  - [ ] A/B testing de elementos clave - *CTAs, navegación, contenido*

- [ ] **Deployment y infraestructura**
  - [ ] Configurar dominio personalizado - *pcbre.com o similar*
  - [ ] Setup SSL certificate - *HTTPS obligatorio*
  - [ ] Configurar CDN (Cloudflare) - *Caching global, protección DDoS*
  - [ ] Setup CI/CD con GitHub Actions - *Deploy automático en push*
  - [ ] Configurar staging environment - *Ambiente de pruebas*
  - [ ] Setup error monitoring (Sentry) - *Tracking de errores en producción*
  - [ ] Configurar Google Analytics 4 - *Métricas de tráfico y uso*
  - [ ] Setup Google Search Console - *Monitoreo SEO*
  - [ ] Crear backup strategy - *Respaldos automáticos*
  - [ ] Documentar proceso de deployment - *README para futuros deploys*

- [ ] **Post-lanzamiento**
  - [ ] Monitorear métricas de performance - *Analytics, Core Web Vitals, uptime*
  - [ ] Recopilar feedback de usuarios - *Formularios, encuestas, comentarios*
  - [ ] Crear plan de contenido continuo - *Nuevas guías, actualizaciones*
  - [ ] Setup newsletter/blog (opcional) - *Noticias de hardware, tips*
  - [ ] Planificar features v2.0 - *Roadmap para próximas versiones*
  - [ ] Crear documentación para mantenimiento - *Cómo actualizar, troubleshooting*

## Stack Tecnológico Propuesto

### Frontend
- **Framework**: React/Next.js o Vue/Nuxt.js
- **Styling**: Tailwind CSS + CSS Modules
- **Build Tool**: Vite o Webpack
- **Animations**: Framer Motion o GSAP

### Herramientas
- **Design**: Figma para mockups
- **Version Control**: Git + GitHub
- **Deployment**: Vercel o Netlify
- **Analytics**: Google Analytics 4

## Estructura de Archivos Propuesta

```
pcbre-v2/
├── public/
│   ├── images/
│   ├── videos/
│   └── icons/
├── src/
│   ├── components/
│   │   ├── common/
│   │   ├── layout/
│   │   └── pages/
│   ├── pages/
│   ├── styles/
│   ├── utils/
│   └── data/
├── docs/
└── tests/
```

## Métricas de Éxito
- **UX**: Tiempo promedio en sitio > 5 minutos
- **Engagement**: Tasa de rebote < 40%
- **Educativo**: Completar flujo completo > 60%
- **Performance**: Core Web Vitals en verde
- **Accesibilidad**: Score WCAG 2.1 AA completo

## Timeline Estimado
- **Fase 1**: 2-3 semanas
- **Fase 2**: 4-5 semanas  
- **Fase 3**: 3-4 semanas
- **Fase 4**: 2-3 semanas

**Total**: 11-15 semanas para MVP completo

## Current Goal
Iniciar Fase 1: Investigación y definición de arquitectura de información