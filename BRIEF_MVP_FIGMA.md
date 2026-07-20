# 🧭 BRIEF MVP — RUTAS SECTOR PÚBLICO × LINKEDIN
**Para uso con Figma IA — Prototipo Animado**
**Versión:** 1.0 | **Fecha:** Julio 2026

---

## 🎯 CONTEXTO DEL PRODUCTO

**Qué es:** Una nueva funcionalidad integrada dentro de LinkedIn que actúa como "Brújula de Carrera Pública" para el mercado colombiano.

**Problema que resuelve:** Los usuarios de LinkedIn no saben si califican para cargos en el sector público, qué les falta para calificar, ni cómo prepararse. La información está dispersa y los requisitos son confusos.

**Propuesta de valor única:** "CV Inverso" — en lugar de que el usuario adapte su CV a la oferta, la plataforma analiza automáticamente su perfil de LinkedIn y le dice exactamente qué le falta para acceder al cargo público que desea.

**Integración con LinkedIn:** La funcionalidad vive dentro del ecosistema LinkedIn como una nueva sección/módulo accesible desde el perfil y desde el tab de "Empleos". Aprovecha el perfil existente del usuario (experiencia, educación, habilidades) para eliminar fricción en la ingesta de datos.

---

## 👥 USUARIO PRIMARIO (para prototipo)

**Arquetipo principal:** Carlos — Profesional con 8+ años en sector privado que quiere transicionar al sector público.
- Motivación: Estabilidad, beneficios, pensión
- Dolor: "Mi experiencia privada no parece contar para los requisitos públicos"
- Dispositivo: Desktop / Mobile (LinkedIn app)

---

## 🗺️ FLUJO UX COMPLETO — 5 PANTALLAS PRINCIPALES

> El flujo está diseñado para completarse en **menos de 10 minutos** y producir un resultado de valor inmediato.

---

### PANTALLA 1 — Entry Point (Discovery / Onboarding)
**Dónde aparece:** Tab "Empleos" de LinkedIn → nueva sección "Sector Público CO" con badge "Nuevo"

**Elementos de UI:**
- Banner destacado con headline: *"¿Listo para el sector público? Descubre qué cargos ya puedes alcanzar"*
- Subheadline: *"Analizamos tu perfil de LinkedIn automáticamente"*
- CTA primario: botón azul LinkedIn → **"Analizar mi perfil"**
- Social proof: *"Más de X profesionales ya conocen su ruta"*
- Badge de credibilidad: logo DAFP + "Datos oficiales"
- Enlace secundario: *"Ver cómo funciona"* (tooltip o modal de 3 pasos)

**Objetivo UX:** Generar confianza y reducir la fricción de entrada. El usuario NO debe crear cuenta nueva.

---

### PANTALLA 2 — Ingesta de Perfil (Confirmación + Complemento)
**Qué hace:** Muestra los datos del perfil de LinkedIn ya importados y pide solo los 3 datos que LinkedIn NO tiene.

**Elementos de UI:**
- Header: *"Confirmamos tu perfil — solo 3 preguntas adicionales"*
- **Sección "Ya tenemos" (solo lectura, con checkmarks verdes):**
  - ✅ Nivel educativo (ej: "Ingeniería de Sistemas — Uniandes")
  - ✅ Años de experiencia (ej: "8 años en sector privado")
  - ✅ Habilidades principales (ej: "Gestión de proyectos, Excel, Liderazgo")
- **Sección "Necesitamos saber" (3 preguntas máximo):**
  1. ¿Qué tipo de cargo público te interesa? → Dropdown: [Nacional / Departamental / Municipal]
  2. ¿Cuál es tu área de interés? → Dropdown: [TI, Salud, Educación, Administración, Jurídico, Otro]
  3. ¿Tienes experiencia previa en entidades públicas? → Toggle Sí / No
- CTA: **"Generar mi análisis"** (barra de progreso animada al hacer clic)

**Objetivo UX:** Demostrar que LinkedIn ya conoce al usuario. Mínima fricción = máxima conversión.

---

### PANTALLA 3 — Análisis de Compatibilidad (Loading + Resultado)
**Estado A — Loading (2-3 segundos):**
- Animación de progreso con micro-copy dinámico:
  - *"Leyendo tu experiencia…"*
  - *"Comparando con 50 cargos públicos…"*
  - *"Calculando tu compatibilidad…"*

**Estado B — Resultado (pantalla principal):**
- Header: *"Tu compatibilidad con el Sector Público"*
- **Score visual central:** Medidor tipo gauge/donut grande con porcentaje (ej: 72%)
  - Verde: 70–100% | Amarillo: 40–69% | Rojo: 0–39%
- **Top 3 cargos compatibles** (cards horizontales scrolleables):
  - Cada card: [Nombre del cargo] + [% compatibilidad] + [Entidad tipo] + [Nivel de salario estimado]
  - CTA por card: *"Ver detalle"*
- **Resumen de fortalezas** (máx. 3 ítems con íconos):
  - ✅ Educación: Cumple requisitos para 80% de cargos
  - ✅ Experiencia: 8 años equivalen al nivel profesional grado 3
  - ⚠️ Sin experiencia en entidades públicas (gap identificado)

**Objetivo UX:** Dar una victoria inmediata al usuario. El score personalizado engancha emocionalmente.

---

### PANTALLA 4 — Reporte de Brecha ("¿Qué me falta?")
**Qué hace:** Para el cargo más compatible seleccionado, muestra exactamente la diferencia entre el perfil actual y los requisitos del cargo.

**Elementos de UI:**
- Header: *"Tu brecha para [Profesional Universitario Grado 3 — TI]"*
- **Tabla de comparación visual (2 columnas):**

  | Requisito del Cargo | Tu Perfil | Estado |
  |---|---|---|
  | Título universitario en TI | Ing. Sistemas | ✅ Cumple |
  | 2 años experiencia relacionada | 8 años | ✅ Supera |
  | Tarjeta profesional COPNIA | No registrada | ⚠️ Pendiente |
  | Conocimiento en contratación pública | No detectado | ❌ Gap crítico |

- **Score de brecha:** *"Estás a 2 pasos de calificar"* (visual de barra casi llena)
- Fuente de datos: *"Basado en Manual de Funciones DAFP — Actualizado [fecha]"* (sello de credibilidad)
- CTA: **"Ver mi plan de preparación"**

**Objetivo UX:** Responder la pregunta clave *"¿Por qué no califico?"* con claridad total. Esto valida H1.

---

### PANTALLA 5 — Recomendaciones (Plan de Acción)
**Qué hace:** Entrega 3–5 acciones concretas, priorizadas y accionables desde LinkedIn.

**Elementos de UI:**
- Header: *"Tu ruta para lograrlo — estimado 4 meses"*
- **Lista de acciones priorizadas (máx. 4 cards):**

  **Card 1 — Acción inmediata (semana 1):**
  - Ícono 🔴 urgente
  - *"Registra tu tarjeta profesional COPNIA"*
  - Subtexto: *"Requisito bloqueante — sin esto no puedes aplicar"*
  - CTA: *"Cómo hacerlo →"* (link externo COPNIA)

  **Card 2 — Corto plazo (mes 1):**
  - Ícono 🟡
  - *"Toma el curso de Contratación Estatal (Ley 80)"*
  - Subtexto: *"Aparece en el 90% de las convocatorias TI"*
  - CTA: *"Ver cursos en LinkedIn Learning →"* (integración nativa)

  **Card 3 — Mediano plazo (mes 2-3):**
  - Ícono 🟢
  - *"Postúlate a convocatoria OPS como primera experiencia pública"*
  - Subtexto: *"Sin concurso de méritos, ideal para ganar experiencia"*
  - CTA: *"Ver convocatorias abiertas →"*

  **Card 4 — Comunidad (siempre disponible):**
  - Ícono 💬
  - *"Conecta con profesionales que ya trabajan en el sector"*
  - Subtexto: *"3 personas en tu red trabajan en el sector público"* (dato de LinkedIn)
  - CTA: *"Ver perfiles →"* (integración con red LinkedIn)

- **CTA final sticky:** *"Guardar mi ruta"* → guarda el plan en el perfil de LinkedIn del usuario

**Objetivo UX:** Hacer que el usuario se vaya con acciones claras. El uso de LinkedIn Learning y la red existente ancla el feature en el ecosistema LinkedIn.

---

## 📐 ESPECIFICACIONES DE DISEÑO PARA FIGMA

### Sistema Visual
- **Usar el Design System de LinkedIn:** Colores, tipografía y componentes nativos de LinkedIn
  - Color primario: `#0A66C2` (LinkedIn Blue)
  - Color de fondo: `#F3F2EF`
  - Tipografía: SF Pro / Inter (la que usa LinkedIn)
  - Bordes de cards: `border-radius: 8px`, sombra suave
- **Colores de estado:**
  - ✅ Verde éxito: `#057642`
  - ⚠️ Amarillo advertencia: `#F5A623`
  - ❌ Rojo gap: `#CC1016`

### Componentes a crear en Figma
1. **Card de cargo público** (con score de compatibilidad)
2. **Gauge/Donut chart** (score general de compatibilidad)
3. **Tabla de brecha** (2 columnas con íconos de estado)
4. **Card de acción** (con prioridad por color)
5. **Banner entry point** (para tab de Empleos)
6. **Modal de confirmación de perfil** (datos pre-llenados)

### Animaciones recomendadas para prototipo
- Pantalla 1 → 2: Slide-up sheet / modal
- Pantalla 2 → 3: Loading animado (3 micro-copy secuenciales) → fade-in al resultado
- Pantalla 3 → 4: Click en card → slide-right al detalle
- Pantalla 4 → 5: CTA → slide-right al plan
- Pantalla 5: Cards que aparecen con stagger (una por una, 100ms de delay)

---

## ✅ QUÉ VALIDA ESTE PROTOTIPO (Hipótesis a testear)

| Hipótesis | Pantalla clave | Indicador de validación |
|---|---|---|
| H1: El usuario entiende por qué no califica | Pantalla 4 (Brecha) | "Ahora entiendo qué me falta" |
| H2: El CV Inverso visual genera confianza | Pantalla 3 (Score) | Tiempo en pantalla > 30s |
| H3: El plan de acción genera intención de actuar | Pantalla 5 (Recomendaciones) | Click en algún CTA |
| H4: Integración LinkedIn reduce fricción | Pantalla 2 (Ingesta) | Completar en < 2 min |

---

## 🚫 FUERA DEL ALCANCE DEL MVP (No prototipar)

- Mentoría 1:1 / modelo premium
- Comunidad y storytelling
- Integración real con DAFP (simular con datos ficticios en el prototipo)
- Sistema de seguimiento de aplicaciones
- Notificaciones push de nuevas convocatorias

---

## 📋 INSTRUCCIÓN PARA FIGMA IA

> Crea un prototipo animado de 5 pantallas para mobile y desktop integrado en LinkedIn. El flujo es: Entry Point en tab Empleos → Confirmación de Perfil (3 preguntas) → Score de Compatibilidad con gauge animado → Tabla de Brecha → Plan de Recomendaciones con 4 cards priorizadas. Usa el design system de LinkedIn (#0A66C2, tipografía Inter, cards con border-radius 8px). Incluye animaciones de transición entre pantallas: slide-up para modales, fade-in para el score tras loading, y stagger para las cards de recomendaciones. El tono es profesional, empático y empoderador. El producto se llama "Rutas Públicas CO" y vive dentro del ecosistema de LinkedIn como una funcionalidad nueva en el tab de Empleos.

---

*Brief generado desde RESUMEN_ESTRATEGICO_PRODUCTO.md | Julio 2026*
