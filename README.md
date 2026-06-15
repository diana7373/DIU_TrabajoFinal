# DIU_TrabajoFinal
Trabajo final DIU 25/26

# PARTE I: Mi experiencia en UI/UX/Usabilidad

**Diana Peven Kobtseva** — DIU 2025/26, grupo DIU3_Juashani — Proyecto "Cyber-Gourmet" (Sabores con Encanto)

## Introducción

A lo largo de la asignatura de Diseño de Interfaces de Usuario (DIU) he aplicado de forma progresiva el ciclo de Diseño Centrado en el Usuario (DCU) descrito en la norma ISO 9241-210: investigar, definir, idear, prototipar y evaluar. Junto a mi compañera Beatriz Ruz Gómez desarrollé el caso de estudio "Cyber-Gourmet", una propuesta de rediseño de la experiencia digital de una hamburguesería gourmet, partiendo del análisis de la web real de Goiko. A continuación repaso las aportaciones más destacadas de cada práctica, valorándolas críticamente y relacionándolas con los conceptos trabajados en clase, y termino con una autovaloración del nivel de experiencia adquirido.

## Práctica 1: Investigación y diagnóstico

Mi primera contribución relevante fue el User Research Plan, donde definimos objetivos medibles: comprobar si un usuario puede seleccionar, personalizar y añadir una hamburguesa al carrito en menos de 50 segundos; validar si los iconos de alérgenos se comprenden sin ayuda; detectar dónde se abandona el checkout; y evaluar si la presentación visual incrementa la intención de compra. Para responderlas diseñamos una metodología combinada —cuantitativa (SEQ, Tree Testing), biométrica (Eye Tracking, análisis facial) y comparativa (benchmarking, First Click Testing)—, lo que me hizo comprender que cada técnica responde a un tipo de pregunta distinto y que combinarlas reduce el sesgo de un único método.

A partir de ahí realizamos una revisión heurística de la web de Goiko con la plantilla de Usability Review (criterios Nielsen), obteniendo 53/100 ("Moderado"). Lo más valioso no fue la cifra, sino aprender a justificar cada valoración con un criterio concreto: calificamos como poco intuitivo que el usuario deba iniciar un pedido e introducir su dirección solo para ver los precios, vinculándolo a la visibilidad del estado del sistema; documentamos la pérdida de datos del carrito al retroceder como una violación de la prevención de errores; y señalamos elementos decorativos que penalizaban el rendimiento sin aportar valor.

Con esa información construimos la persona "Nanami Momozono", una creadora de contenido japonesa de 27 años que visita Granada y necesita pedir comida rápida y vistosa para sus redes sociales en un idioma que no domina del todo. Crear esta persona me enseñó que no es un perfil demográfico decorativo, sino una herramienta de priorización: de Nanami se derivaron necesidades concretas (rapidez, soporte multilingüe, estética del producto) que condicionaron decisiones posteriores. El Customer Journey Map asociado, estructurado en las fases Awareness–Inspiration–Decide–Act–Observation, nos permitió visualizar expectativas y emociones en cada paso, conectando la investigación cualitativa con la arquitectura de la información de la práctica siguiente.

## Práctica 2: Ideación y arquitectura de la información

Mi aportación más directa fue el Mapa de Empatía de Nanami, donde recogí afirmaciones como "me gusta el sabor de las hamburguesas", "es una comida muy calórica" o "buena comida para generar vistas". Analizar estas frases me permitió identificar una tensión no evidente en la persona inicial: el usuario quiere disfrutar la comida y compartirla en redes, pero también le preocupa su imagen pública y el aporte calórico. Esa tensión se convirtió en el insight del proyecto: no bastaba con vender hamburguesas, había que ofrecer una experiencia memorable y "compartible".

Formalizamos ese insight en el Value Proposition / Scope Canvas, traduciendo los dolores del usuario (dificultad para elegir entre muchas opciones, falta de personalización online, webs poco interactivas) y sus motivadores (personalizar su hamburguesa, participar en rankings, sentirse parte de una comunidad) en un propósito de marca: "transformar la web en una experiencia interactiva, social y memorable, donde los usuarios no solo compren hamburguesas, sino que las creen, las compartan y formen parte de la marca", con métricas concretas asociadas (reseñas en Google, hamburguesas creadas por usuarios, engagement en redes). Este canvas me hizo entender la diferencia entre una "buena idea" y una propuesta de valor accionable.

Esa propuesta se trasladó al Sitemap: junto a las secciones habituales (Carta, Realizar pedido, Contacto, Reservar, Sobre Nosotros), incorporamos "Personalización de hamburguesas" con su propio ranking de creaciones y la opción de sugerir nuevos ingredientes, respondiendo directamente a los motivadores del mapa de empatía. Esto me hizo ver la arquitectura de la información no como una lista de páginas, sino como la materialización estructural de la propuesta de valor. Los wireframes de baja fidelidad fijaron la jerarquía de contenidos sin entrar en decisiones visuales, en línea con el modelo de los "cinco planos" de Garrett: primero el esqueleto antes que la superficie.

## Práctica 3: Identidad visual y diseño de la interfaz

En esta práctica definimos la identidad "Cyber-Gourmet": un moodboard con paleta morado/verde neón/rojo/negro, tipografía "Press Start 2P" (pixel art) para titulares y "Average Sans" para el cuerpo, y un vocabulario propio de videojuegos (Build Mode, "Level: Artisan", "Hackear el menú") coherente con el insight de Nanami. Mi aportación se centró en justificar estas decisiones más allá del gusto estético: el alto contraste entre el fondo negro y los acentos neón crea una jerarquía visual que dirige la mirada hacia los Call to Action, aplicando los principios de contraste y figura-fondo trabajados en clase.

Una parte especialmente formativa fue el uso de IA generativa (Figma Make) para producir la Landing Page a partir de un prompt detallado, especificando modo oscuro, tipografía, paleta y estructura de contenidos. Esto me hizo ver que el prompting para diseño es, en el fondo, una especificación de requisitos: si no se concreta cada decisión, la IA recurre a patrones genéricos que no representan la marca, reforzando la importancia de tener un moodboard y un design system sólidos antes de delegar trabajo en herramientas generativas.

El Design System lo abordamos siguiendo Atomic Design (Brad Frost): definimos átomos (inputs de texto, botones con distintos estados, paleta de color y escalas tipográficas) y desarrollamos los suficientes componentes para demostrar el criterio de consistencia. En el Layout Hi-Fi ensamblamos esos átomos en pantallas finales aplicando Auto Layout para garantizar la adaptabilidad responsiva, experimentando de primera mano el salto de "elemento aislado" a "sistema coherente".

## Práctica 4: Prototipado funcional y desarrollo

En esta práctica migramos el diseño de Figma a un proyecto real con Vite + React, Tailwind CSS y componentes de shadcn/ui. Mi contribución se centró en comprobar que los átomos definidos en la práctica anterior podían trasladarse a clases de utilidad de Tailwind de forma centralizada, aplicando la estética "neobrutalista/arcade" (bordes gruesos, sombras direccionales, alto contraste) de manera sistemática en toda la interfaz.

El resultado fueron dos prototipos funcionales: la Landing Page (con el hero "Diseñada por ti, perfeccionada por el fuego") y el formulario "Construye tu Arsenal", que organiza la personalización de la hamburguesa en bloques (Pan, Proteína, Queso, Toppings, Salsas, Nivel de picante) y muestra en tiempo real un panel con el resumen del pedido. Esta práctica fue la que más me hizo valorar las decisiones anteriores: un sitemap y un design system bien definidos convirtieron la implementación en una traducción técnica del trabajo de diseño y no en un rediseño sobre la marcha. También aprendí que un componente que "se ve bien" en Figma puede comportarse de forma distinta cuando tiene estados reales (hover, selección, foco), algo que identificamos como mejora pendiente.

## Práctica 5: Evaluación, usabilidad y accesibilidad

La última práctica fue la más reveladora, porque puso a prueba con datos todas las decisiones anteriores. Participé en el reclutamiento de 10 usuarios con perfiles, experiencia tecnológica y "situaciones de conflicto" muy distintas. Cinco evaluaron nuestro Caso A (Cyber-Gourmet) y otros cinco el Caso B asignado (Punto Café).

Los resultados del cuestionario SUS (System Usability Scale, Brooke, 1996) fueron un toque de humildad: Cyber-Gourmet obtuvo una media de 73,75 puntos ("Aceptable"), frente a 82,5 del Caso B. Nuestra propuesta —más ambiciosa visual y conceptualmente— resultó menos usable que una más convencional. Cruzar esta cifra con el Eye Tracking (mapas de calor de la Landing y del formulario) ayudó a entender por qué: la atención se concentraba en el hero y en las imágenes de producto, pero la jerga "gamer" (Build Mode, Daily Quests, Top Players) y la tipografía pixelada generaban fricción cognitiva, especialmente para perfiles poco familiarizados con los videojuegos. Esta es una de las lecciones más importantes de la asignatura: diferenciarse visualmente no debe hacerse a costa de la usabilidad.

Como parte del intercambio entre grupos, realicé la auditoría de accesibilidad (WCAG 2.1, nivel AA) del proyecto "Punto Café", según los principios POUR (Perceptible, Operable, Comprensible, Robusto): déficit de contraste en placeholders (criterio 1.4.3), tipografía decorativa en botones (1.4.8), iconos de redes sin aria-label (2.4.4) y campos de entrada sin área clicable clara (3.3.2), con Lighthouse estimado en 65/100. Priorizar estos hallazgos me obligó a pasar de "esto no se ve bien" a "esto incumple el criterio X de WCAG y afecta a usuarios con Y condición". Aplicando esta misma lista a Cyber-Gourmet detecté que la tipografía "Press Start 2P" en los CTA y el contraste neón sobre negro arrastrarían problemas similares, algo a priorizar en una futura iteración.

## Trabajos teóricos complementarios

Además del caso de estudio, varios ejercicios teóricos enriquecieron mi formación. La evaluación heurística de distintas universidades españolas me permitió aplicar criterios basados en Nielsen y leyes de interacción como las de Fitts, Hick y Miller, aprendiendo a justificar cada observación mediante principios concretos y evitando valoraciones subjetivas.

También participé en el desarrollo conceptual de Cat-feína, una propuesta de cafetería temática con gatos, donde trabajé la construcción de identidad visual mediante moodboards, selección de paletas cromáticas y tipografías coherentes con el público objetivo. Por último, la elaboración de mi portfolio personal me obligó a reflexionar sobre la jerarquía visual, la claridad de navegación y la comunicación efectiva de proyectos, aplicando los mismos criterios de diseño centrado en el usuario trabajados en las prácticas principales.

## Autovaloración final

Si tuviera que resumir el nivel de experiencia adquirido, diría que parto de una base sólida en las fases de investigación y conceptualización (research plan, personas, journey maps, mapas de empatía, value proposition canvas) y de diseño visual y prototipado (moodboards, design systems con Atomic Design, wireframes, layouts Hi-Fi e implementación funcional en React/Tailwind). Sé plantear objetivos de investigación medibles, traducir insights cualitativos en decisiones de arquitectura de la información y llevar un diseño desde Figma hasta un prototipo funcional manteniendo coherencia con un sistema de componentes.

Mi punto más débil, y a la vez mi mayor aprendizaje, está en la fase de evaluación: los resultados de SUS, Eye Tracking y accesibilidad demostraron que una propuesta visualmente diferenciadora puede introducir, sin pretenderlo, barreras que solo se detectan probando con usuarios reales y aplicando checklists normativas. Antes de esta práctica tendía a valorar un diseño por su impacto visual; ahora sé que ese impacto debe contrastarse con datos de uso y criterios verificables, y que "diseñar diferente" y "diseñar usable" no son sinónimos, aunque tampoco objetivos contrapuestos si se itera con esa información.

Considero que he alcanzado un nivel intermedio-avanzado en investigación, personas, journey maps, design systems y prototipado (incluyendo IA generativa), y un nivel intermedio en evaluación de usabilidad y accesibilidad. Esta última es precisamente el área en la que me propongo seguir formándome: integrar revisiones de accesibilidad y pruebas con usuarios desde las primeras fases del proceso, y no solo al final, como ocurrió con Cyber-Gourmet.


# PARTE II: Caso de Estudio — Propuesta de Diseño para el Ecomercado UGR

**Diana Peven Kobtseva** | DIU 2025/26 | Grupo DIU3_Juashani

---

## 1. Contexto del caso

El **Ecomercado UGR** es una iniciativa inaugurada el 26 de marzo de 2026 en los Paseíllos del Campus de Fuentenueva, impulsada por la Universidad de Granada y la Red Agroecológica de Granada. Se celebra el cuarto jueves de cada mes (9:30–14:00 h) y reúne a una quincena de productores locales (Somos Vega Somos Tierra, Cooperativa Valle y Vega, La Zarzamora, entre otros) bajo el paraguas del *Living Lab* **Granada Tierra Viva** (proyecto europeo SOILCRATES). Su propósito trasciende lo comercial: busca ser un espacio de sensibilización y conexión entre campo y ciudad.

A fecha del análisis, el Ecomercado UGR **carece de presencia digital propia**: sin app ni web dedicada, la información se distribuye exclusivamente por redes sociales y medios institucionales. Este vacío es la oportunidad de diseño que aborda este informe.

---

## 2. Análisis del referente: Nuestras Huertas (nuestrashuertas.com)

**Nuestras Huertas Sierra Norte** (Bustarviejo, Madrid) lleva más de diez años ofreciendo productos ecológicos certificados con reparto a domicilio, puntos de recogida y mercado presencial. Dispone de tienda online y blog.

### 2.1 Revisión heurística (Nielsen)

| # | Heurística | Punt. (0–4) | Observación |
|---|-----------|------------|-------------|
| H1 | Visibilidad del estado | 3 | Carrito claro; sin disponibilidad en tiempo real |
| H2 | Correspondencia con el mundo real | 3 | Lenguaje cercano; vocabulario técnico para no iniciados |
| H3 | Control y libertad | 2 | Pedido por Excel + email rompe el flujo digital |
| H4 | Consistencia | 2 | Tienda online y Excel coexisten de forma confusa |
| H5 | Prevención de errores | 2 | Sin validación ni aviso de agotados en el Excel |
| H6 | Reconocimiento vs. recuerdo | 3 | Productos con imagen y nombre reconocibles |
| H7 | Flexibilidad y eficiencia | 2 | Sin búsqueda ni filtros por temporada |
| H8 | Diseño minimalista | 2 | Homepage densa; CTA principal diluido |
| H9 | Ayuda ante errores | 2 | Sin mensajes de error; soporte solo por email |
| H10 | Ayuda y documentación | 3 | Sección "Cómo comprar" clara |

**Puntuación global estimada: 52/100 — Moderado/Mejorable.**

### 2.2 Accesibilidad (WCAG 2.1 AA — principios POUR)

| Principio | Hallazgo |
|-----------|---------|
| **Perceptible** | Contraste insuficiente en menú secundario (ratio < 4.5:1, criterio 1.4.3); imágenes sin `alt` descriptivo (1.1.1) |
| **Operable** | Áreas clicables < 44×44 px en algunos botones (2.5.5) |
| **Comprensible** | Bifurcación tienda/Excel sin señalización clara (3.3.2) |
| **Robusto** | Sin `aria-label` en iconos de redes y carrito (4.1.2) |

**Lighthouse estimado: 58–65/100.**

### 2.3 Insights transferibles al Ecomercado UGR

> **Insight 1 — Transparencia = confianza:** mostrar quién produce, cómo y dónde es diferencial en mercados ecológicos; la identidad del productor debe ser protagonista.

> **Insight 2 — El flujo de pedido es el mayor cuello de botella:** cualquier fricción (Excel, email, llamada) expulsa al usuario digital, especialmente desde móvil.

> **Insight 3 — El calendario es información crítica:** saber qué habrá antes de ir reduce la incertidumbre y aumenta la intención de asistencia.

> **Insight 4 — El público universitario tiene expectativas digitales altas:** una interfaz desactualizada genera desconfianza en la calidad del propio producto.

---

## 3. Propuesta de valor para el Ecomercado UGR

### 3.1 Persona

**Lucía Mármol**, 22 años, estudiante de Biología en la UGR. Vive en piso compartido, se mueve en bici, le preocupa el origen de los alimentos. El móvil es su primer dispositivo para todo. No tiene coche y los jueves tiene clase si no lo planifica con antelación.

**Necesidades clave:** saber qué habrá en el mercado antes del día; poder reservar si va a llegar tarde; conocer la historia de cada productor; recibir recordatorios sin buscar activamente.

### 3.2 Value Proposition Canvas

| Dolor del usuario | Acción propuesta | Métrica |
|------------------|-----------------|---------|
| No sabe qué habrá hasta que llega | Catálogo digital previo por edición | % de usuarios que visitan el catálogo antes del día |
| Llega tarde y no encuentra producto | Pre-reserva con recogida en el puesto | Nº de reservas por edición |
| No conoce a los productores | Fichas de productor con historia y valores | Tiempo en fichas de productor |
| No se entera de la fecha | Recordatorio push/email | Tasa de apertura |

**Propósito:** *"Conectar a la comunidad universitaria con los productores agroecológicos de Granada, haciendo del Ecomercado UGR una experiencia accesible y anticipable, tanto si puedes venir como si no."*

### 3.3 Arquitectura de la información (Sitemap — App móvil)

```
Ecomercado UGR (App)
├── Inicio · próxima edición + CTA "Quiero ir" / "Reservar"
├── Productores · listado con filtro por tipo y comarca
│   └── Ficha de productor (historia, certificaciones, productos)
├── Catálogo · filtro por temporada / tipo / productor
│   └── Detalle de producto → [Reservar]
├── Mi reserva · resumen + confirmación de recogida
├── Ediciones anteriores · archivo por edición
└── Sobre el Ecomercado · qué es · cómo participar
```

### 3.4 Boceto (flujo principal — App móvil)

La propuesta se orienta a **app móvil** porque el perfil dominante (universitario, 18–30 años) accede principalmente desde smartphone y la periodicidad mensual justifica notificaciones *push*.

```
┌─────────────────────────────┐   ┌─────────────────────────────┐
│  🌿 ECOMERCADO UGR          │   │  🛒 Catálogo · Junio 2026   │
│  Jueves 26 jun · 9:30–14h   │   │  [Verdura] [Fruta] [Otro]   │
│  Paseíllos de Fuentenueva   │   │                             │
│                             │   │  🥕 Zanahorias baby         │
│  [Ver catálogo]             │   │     La Zarzamora · Órgiva   │
│  [Conoce los productores]   │   │     [+ Info]  [Reservar]    │
│                             │   │                             │
│  ⏰ Faltan 11 días          │   │  🍅 Tomate rama             │
│  [Activar recordatorio]     │   │     Somos Vega Somos Tierra │
│                             │   │     [+ Info]  [Reservar]    │
└─────────────────────────────┘   └─────────────────────────────┘

┌─────────────────────────────┐   ┌─────────────────────────────┐
│  [← Volver]                 │   │  🛍 Mi reserva              │
│  La Zarzamora               │   │                             │
│  📍 Órgiva, Alpujarra       │   │  Zanahorias baby x1 — 1,5€ │
│                             │   │  Tomate rama   x2 — 3,0€   │
│  ✅ Certificación ecológica │   │                             │
│  🌱 Producción propia       │   │  Recogida: jue 26 jun 9:30  │
│                             │   │                             │
│  En esta edición:           │   │  [Confirmar reserva]        │
│  · Zanahorias · Remolacha   │   │  (Se abona en el puesto)    │
│  [Reservar productos]       │   │                             │
└─────────────────────────────┘   └─────────────────────────────┘
```

---

## 4. Justificación de decisiones de diseño

Cada decisión se vincula a un principio concreto, sin valoraciones subjetivas:

- **Nielsen H1 (Visibilidad del estado):** la cuenta atrás en el inicio garantiza que el usuario siempre sepa cuándo es el próximo mercado, resolviendo el problema detectado en el referente.
- **Nielsen H5 (Prevención de errores):** la reserva sin pago previo elimina la fricción del Excel y permite cancelar sin consecuencias; la selección guiada evita errores de relleno.
- **Nielsen H6 (Reconocimiento vs. recuerdo):** las fichas de productor muestran toda la información relevante en el momento de decisión; el usuario no necesita recordar quién vende qué.
- **Ley de Hick:** los filtros por categoría reducen las opciones visibles simultáneamente, acortando el tiempo de decisión para un usuario que dispone de tiempo limitado.
- **WCAG 2.1 AA:** la propuesta incorpora desde el inicio contraste > 4.5:1, áreas táctiles ≥ 44×44 px y etiquetas ARIA en elementos de acción, corrigiendo los déficits detectados en el referente.
- **ISO 9241-210 (DCU):** la persona y el Value Proposition Canvas aseguran que cada funcionalidad responde a una necesidad real medible, no a una preferencia del diseñador.

---

## 5. Autoevaluación: prácticas y transferencia al caso real

### 5.1 Técnicas aplicadas

| Técnica | Práctica origen | Uso en este caso |
|---------|----------------|-----------------|
| Revisión heurística (Nielsen) | P1 | Análisis de Nuestras Huertas con criterio por ítem |
| Persona | P1 | Lucía Mármol → funcionalidades concretas |
| Insights / Mapa de empatía | P2 | Tensión anticipación vs. incertidumbre |
| Value Proposition Canvas | P2 | Dolor → acción → métrica |
| Sitemap | P2 | Arquitectura orientada a la propuesta de valor |
| Wireframes baja fidelidad | P3 | Bocetos de las 4 pantallas del flujo principal |
| Auditoría WCAG (POUR) | P5 | Análisis del referente + decisiones de diseño accesible |

### 5.2 Qué hubiera sido interesante aplicar

**Card Sorting y Tree Testing:** el sitemap se elaboró a partir del análisis, pero no se validó con usuarios reales. Un card sorting con 10–15 personas del perfil universitario habría verificado si la categorización del catálogo responde a sus modelos mentales.

**Pruebas de usabilidad con usuarios:** los bocetos no han sido testeados. Como aprendí en P5, un diseño que parece claro en papel puede generar fricción real; un test con 5 usuarios habría validado si el flujo de reserva es intuitivo.

**Prototipo Hi-Fi y Design System:** el paso lógico sería un sistema de componentes coherente con la identidad visual de la UGR (verde institucional, tipografía accesible) y un prototipo en Figma para pruebas con interacciones reales.

### 5.3 Reflexión final

La diferencia entre Cyber-Gourmet y el Ecomercado UGR es que el segundo tiene usuarios reales, productores reales y un contexto institucional que condiciona las decisiones. Lo que las prácticas de DIU me aportaron es un **método**: no empezar por la interfaz sino por la investigación, no decidir por gusto sino por criterio verificable, y no dar el diseño por terminado hasta probarlo con datos. La lección que traslado directamente: diferenciarse visualmente y ser usable no son objetivos opuestos, pero el segundo debe preceder siempre al primero.

---

## Referencias

- Nielsen, J. (1994). *10 Usability Heuristics for User Interface Design*. NNGroup.
- W3C. (2018). *Web Content Accessibility Guidelines (WCAG) 2.1*. https://www.w3.org/TR/WCAG21/
- Garrett, J. J. (2011). *The Elements of User Experience* (2ª ed.). New Riders.
- ISO 9241-210:2019. *Human-centred design for interactive systems*.
- Canal UGR. (2026, 26 de marzo). *Primer Ecomercado UGR junto a la Red Agroecológica de Granada*. https://canal.ugr.es
- Nuestras Huertas Sierra Norte. (2025). *nuestrashuertas.com* [Sitio web analizado].
