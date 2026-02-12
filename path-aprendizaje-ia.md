# Path de Aprendizaje: IA aplicada construyendo un proyecto real

## Contexto
- **Quién sos:** PM, ingeniero en sistemas, 6 meses exp dev (C#, Angular, TS, SQL)
- **Objetivo:** Aprender IA como herramienta de desarrollo construyendo un proyecto de 0 a 100
- **Proyecto elegido:** Plataforma EdTech de cursos de producto
- **Primer hito:** Landing page con analytics, construida 100% con IA
- **Disponibilidad:** 10+ horas/semana
- **Mercado inicial:** Córdoba → Buenos Aires

---

## Fase 1: Setup del entorno (Semana 1)

### Qué vas a aprender
- Configurar tu entorno de desarrollo con IA
- Entender cómo Claude Code funciona desde la terminal
- Conectar MCPs a herramientas reales
- Crear tu primer proyecto desde cero con IA

### Tareas

**1.1 — Herramientas base (ya tenés la mayoría)**
- [ ] VSCode instalado y funcionando ✅
- [ ] Ubuntu con Claude Code en terminal ✅
- [ ] Cuenta de GitHub (crear repo para el proyecto)
- [ ] Cuenta de Claude Pro (si no la tenés, $20 USD/mes)

**1.2 — Configurar Claude Code como tu herramienta principal**
- [ ] Abrir terminal Ubuntu
- [ ] Verificar que Claude Code funciona: `claude --version`
- [ ] Crear carpeta del proyecto: `mkdir edtech-landing && cd edtech-landing`
- [ ] Iniciar Claude Code dentro del proyecto: `claude`
- [ ] Tu primer prompt real: pedirle a Claude Code que inicialice un proyecto web

**1.3 — Configurar MCPs útiles**
- [ ] MCP de filesystem (para que Claude Code lea/escriba archivos)
- [ ] MCP de GitHub (para commits y push desde Claude)
- [ ] Opcional: MCP de Notion (si usás Notion para organizar)

**1.4 — Entender el workflow**
- [ ] Practicar el ciclo: prompt → código generado → revisar → iterar
- [ ] Aprender a dar contexto efectivo (qué querés, para qué, restricciones)
- [ ] Experimentar con diferentes niveles de especificidad en prompts

### Conceptos que vas a aprender en esta fase
- Cómo funciona Claude Code vs Claude web (agente con acceso a tu filesystem vs chat)
- Qué es un MCP en la práctica (no solo en teoría)
- El flujo de trabajo real de "vibe coding": describir → generar → iterar
- Git básico desde terminal (init, add, commit, push)

### Entregable
Un repositorio en GitHub con la estructura inicial del proyecto, creado 100% desde Claude Code.

---

## Fase 2: Construir la landing (Semanas 2-3)

### Qué vas a aprender
- Generar frontend completo con IA
- Prompting efectivo para código (ser específico, dar contexto, iterar)
- HTML, CSS, JavaScript moderno (o React si preferís)
- Responsive design
- Buenas prácticas de estructura de proyecto

### Tareas

**2.1 — Definir qué va en la landing (antes de escribir código)**
- [ ] Headline: propuesta de valor clara
- [ ] Secciones: hero, para quién es, qué vas a aprender, formato, precio tentativo, CTA
- [ ] CTA principal: formulario de captura de email ("Anotate en la lista de espera")
- [ ] Definir estilo visual (minimalista, tech, colores)

**2.2 — Generar la landing con Claude Code**
- [ ] Prompt inicial: describir la landing completa y pedirle que la genere
- [ ] Iterar sección por sección (no intentar todo perfecto de una)
- [ ] Aprender a pedir cambios específicos ("hacé el hero más grande", "cambiá la tipografía")
- [ ] Agregar responsive (que se vea bien en mobile)

**2.3 — Formulario de captura de emails**
- [ ] Elegir servicio para capturar emails: Formspree (gratis, simple) o EmailOctopus (gratis hasta 2500 subs)
- [ ] Integrar el formulario en la landing
- [ ] Testear que los emails lleguen

**2.4 — Revisar y pulir**
- [ ] Testear en mobile (Chrome DevTools → toggle device)
- [ ] Revisar velocidad de carga
- [ ] Verificar que el formulario funciona
- [ ] Hacer commit y push a GitHub

### Prompts que vas a practicar
- Prompts descriptivos ("creá una landing para X con estas secciones...")
- Prompts iterativos ("cambiá solo el header, manteniendo el resto igual")
- Prompts de debugging ("el formulario no envía, acá está el error...")
- Prompts con contexto ("estoy usando HTML puro sin framework, tené eso en cuenta")

### Entregable
Landing page funcional en tu repo de GitHub, con formulario de captura de emails funcionando.

---

## Fase 3: Deploy e infraestructura (Semana 3-4)

### Qué vas a aprender
- Qué es hosting, DNS, dominio
- Deploy de un sitio estático
- Infraestructura básica real
- Usar IA para resolver problemas de infra

### Tareas

**3.1 — Comprar dominio**
- [ ] Elegir nombre (algo corto, memorable)
- [ ] Comprarlo en Namecheap o similar (~$10 USD/año)

**3.2 — Deploy**
- [ ] Opción recomendada: Vercel (gratis para proyectos personales)
  - Conectás tu repo de GitHub
  - Cada push hace deploy automático
  - HTTPS gratis incluido
- [ ] Alternativas: Netlify, GitHub Pages, Cloudflare Pages (todas gratis)

**3.3 — Configurar dominio custom**
- [ ] Apuntar DNS del dominio a Vercel
- [ ] Verificar que funcione con HTTPS
- [ ] Entender qué es DNS, A record, CNAME (pedile a Claude que te explique mientras configurás)

**3.4 — Hacer todo desde Claude Code**
- [ ] Pedirle a Claude Code que te guíe el deploy paso a paso
- [ ] Usar la terminal para todo lo posible (Vercel CLI, git push)

### Conceptos que vas a aprender en esta fase
- Hosting estático vs dinámico
- DNS: cómo un dominio se conecta con un servidor
- CI/CD básico: push a GitHub → deploy automático
- HTTPS y SSL

### Entregable
Landing desplegada en internet con dominio propio, accesible para cualquier persona.

---

## Fase 4: Analytics y tracking (Semana 4)

### Qué vas a aprender
- Google Analytics 4 (setup y configuración)
- Meta Pixel (para ads de Facebook/Instagram)
- Event tracking (medir acciones específicas)
- Conceptos de analítica web

### Tareas

**4.1 — Google Analytics 4**
- [ ] Crear cuenta de GA4 (gratis)
- [ ] Obtener el ID de medición
- [ ] Integrar el script en la landing (pedile a Claude Code que lo agregue)
- [ ] Verificar que trackea visitas en tiempo real

**4.2 — Meta Pixel**
- [ ] Crear cuenta de Meta Business Suite (gratis)
- [ ] Crear un pixel
- [ ] Agregar el código a la landing
- [ ] Configurar evento "Lead" cuando alguien deja su email
- [ ] Verificar con Meta Pixel Helper (extensión de Chrome)

**4.3 — Eventos custom**
- [ ] Trackear: visitas, scroll depth, clicks en CTA, formulario enviado
- [ ] Configurar estos eventos tanto en GA4 como en Meta Pixel
- [ ] Aprender la diferencia entre pageview, evento y conversión

**4.4 — Opcional: Hotjar**
- [ ] Cuenta gratis (35 sesiones/día)
- [ ] Ver grabaciones de cómo la gente interactúa con tu landing
- [ ] Heatmaps de dónde hacen click

### Conceptos que vas a aprender en esta fase
- Cómo funciona el tracking web (scripts, cookies, eventos)
- GA4: métricas, dimensiones, reportes
- Meta Pixel: cómo Facebook trackea usuarios para ads
- Event-driven analytics vs pageviews

### Entregable
Landing con GA4 + Meta Pixel funcionando, trackeando visitas y conversiones (emails capturados).

---

## Fase 5: Ads y validación (Semanas 5-6)

### Qué vas a aprender
- Meta Ads Manager (crear campañas)
- Segmentación de audiencia
- A/B testing básico
- Interpretar métricas de ads
- Tomar decisiones basadas en datos

### Tareas

**5.1 — Preparar assets para ads**
- [ ] 2-3 variantes de copy (texto del anuncio)
- [ ] 2-3 variantes de visual (imagen o video corto)
- [ ] Podés usar IA para generar los copies y las imágenes

**5.2 — Configurar campaña en Meta Ads**
- [ ] Objetivo: Conversiones (leads)
- [ ] Audiencia: Córdoba, 22-35, intereses en producto/tech/startups
- [ ] Presupuesto: $5-10 USD/día, 2 semanas
- [ ] A/B test: probar diferentes copies/visuales

**5.3 — Monitorear y optimizar**
- [ ] Revisar métricas diarias: impresiones, clicks, CTR, CPC, conversiones
- [ ] Pausar ads que no funcionan
- [ ] Escalar los que sí

**5.4 — Evaluar resultados**
- [ ] Tasa de conversión landing (visitas → emails)
- [ ] Costo por lead
- [ ] Cantidad total de leads
- [ ] Decidir: ¿hay demanda real? ¿sigo, pivoteo o itero la propuesta?

### Entregable
Campaña corrida, datos recolectados, decisión tomada sobre el siguiente paso.

---

## Fase 6: Siguiente paso (Semana 7+)

Dependiendo de los resultados de la validación:

**Si hay demanda (>10% conversión, leads entusiasmados):**
→ Construir la plataforma real. Acá es donde usás todo lo aprendido para hacer back-end, base de datos, auth, API, etc. con IA.

**Si hay demanda tibia (3-10% conversión):**
→ Iterar la propuesta. Cambiar el ángulo, el nicho, el formato. Correr otra ronda de ads.

**Si no hay demanda (<3% conversión):**
→ Pivotar a otro producto. Pero ya tenés todo el stack aprendido: Claude Code, MCPs, deploy, analytics, ads. Podés construir cualquier cosa.

---

## Resumen del stack que vas a dominar

| Herramienta | Para qué |
|---|---|
| Claude Code | Generar código, resolver problemas, guiar desarrollo |
| VSCode | Editor de código |
| Git/GitHub | Control de versiones y repo |
| MCPs | Conectar Claude a filesystem, GitHub, etc. |
| HTML/CSS/JS | Frontend de la landing |
| Vercel | Deploy y hosting |
| GA4 | Analytics web |
| Meta Pixel | Tracking para ads |
| Meta Ads | Campañas de publicidad |
| Formspree/EmailOctopus | Captura de leads |

## Inversión estimada

| Item | Costo |
|---|---|
| Claude Pro | $20 USD/mes |
| Dominio | ~$10 USD/año |
| Hosting (Vercel) | Gratis |
| GA4 | Gratis |
| Meta Pixel | Gratis |
| Ads (2 semanas) | $70-140 USD |
| Formspree | Gratis |
| **Total primer mes** | **~$100-170 USD** |

---

## Reglas del path

1. **Todo se hace con IA.** Si podés pedírselo a Claude Code, no lo hagas manual.
2. **Aprendé haciendo.** No estudies Git 3 horas antes de usarlo. Usalo y preguntale a Claude cuando te trabes.
3. **Iterá rápido.** La landing no tiene que ser perfecta. Tiene que existir.
4. **Documentá lo que aprendés.** Cada concepto nuevo que entiendas, anotalo. Te va a servir para la plataforma real después.
5. **Preguntá acá.** Este proyecto Claude es tu espacio de trabajo. Volvé con dudas, errores, decisiones.
