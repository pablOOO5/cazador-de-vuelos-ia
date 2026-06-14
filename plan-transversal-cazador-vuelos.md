# Cazador de Vuelos — Plan transversal

> **Nota:** el carrusel viral y la guía de prompts (keyword VUELO) ya se publicaron y entregaron. Este repositorio es la **evolución a skill**: la misma lógica, ahora estructurada y lista para instalar. Este documento explica la estrategia de los 4 niveles que da forma al producto.

Una sola herramienta, cuatro niveles de usuario. La idea: cualquiera —desde el que abre ChatGPT gratis hasta el dev que lo integra en Claude Code— puede cazar vuelos baratos con la misma lógica. Cambia el envase, no el contenido.

El objetivo de fondo para todos: **ahorrar plata y tiempo, y ver lo que el viajero promedio no ve** (aerolíneas ocultas, costos escondidos, letra chica).

---

## Mapa rápido

| Nivel | Para quién | Formato | Dónde |
|---|---|---|---|
| 1 | Usa IA como chat, no sabe qué es un skill | 1 prompt maestro (copiar y pegar) | ChatGPT, Gemini, Copilot, Claude (gratis) |
| 2 | Ya copia prompts, quiere control por etapa | Pedidos por módulo (lenguaje natural) | Cualquier chat de IA |
| 3 | Usuario Claude que quiere que sea automático | Skill cargado | Claude.ai (pago) y Claude Cowork |
| 4 | Técnico / dev, lo integra a su flujo | Skill instalado + datos reales | Claude Code (y Cursor, Codex CLI) |

La regla de oro vale en los 4 niveles: **nunca inventar precios ni códigos. Verificar con búsqueda web cuando se pueda, y marcar qué es dato confirmado y qué es estimación.**

---

## Nivel 1 — El que usa el chat y nada más

**Para quién:** la mayoría. Abre ChatGPT, Gemini o Claude gratis, escribe y listo. No instala nada.

**Qué recibe:** el [prompt maestro](usar-sin-skill/prompt-maestro.md) que hace todo el trabajo de una. Solo tiene que reemplazar lo que está entre corchetes y **activar la búsqueda web** del modelo.

**Cómo lo usa:** copia, pega, completa los datos, manda. Guía: [`guias/chatgpt-gemini-claude-free.md`](guias/chatgpt-gemini-claude-free.md).

**Límite honesto:** si el modelo no tiene búsqueda web activa, va a estimar. Por eso el prompt le exige marcar qué es estimación. Sin web, sirve para orientarse; con web, para decidir.

---

## Nivel 2 — El que quiere control por etapa

**Para quién:** el que prefiere ir paso a paso, o solo necesita una parte (ej: nada más el mail de negociación).

**Qué recibe:** la capacidad de pedir cualquiera de los 8 módulos suelto, en lenguaje natural. Cada uno resuelve una etapa: fechas óptimas, aerolíneas ocultas, escalas, promos, costos ocultos, mail de negociación, flexibilidad/riesgo, hidden city ticketing.

**Ejemplo:** ya tiene dos opciones de vuelo y solo quiere saber cuál es menos riesgosa → pide únicamente el módulo de *flexibilidad y riesgo*, pega las dos opciones, y le pide que marque la letra chica.

---

## Nivel 3 — El usuario Claude que quiere que sea automático

**Para quién:** el que usa Claude.ai pago o Claude Cowork y no quiere copiar y pegar nada. Quiere escribir "encontrame vuelos a X" y que pase solo.

**Qué recibe:** el skill `vuelos-baratos`. Guía: [`guias/claude-ai-skill.md`](guias/claude-ai-skill.md).

**Ejemplo:** *"Encontrame vuelos baratos de Buenos Aires a Madrid en septiembre, tengo 4 días de flexibilidad y me importa más el precio que el tiempo."* Claude corre el pipeline entero sin que el usuario sepa que hay 8 módulos detrás.

**Ventaja vs. Nivel 1:** no depende de que el usuario sepa prompts. La experiencia es "le hablo y resuelve".

---

## Nivel 4 — El técnico que lo integra a su flujo

**Para quién:** dev o power user. Lo versiona, lo mejora, lo conecta a datos reales.

**Qué recibe:** el mismo skill, instalado a nivel sistema. Guía: [`guias/claude-code-skill.md`](guias/claude-code-skill.md).

**Cómo lo usa:**
- Pone la carpeta `vuelos-baratos/` en `~/.claude/skills/`, abre una sesión de Claude Code y verifica con `/skills`.
- El formato SKILL.md es estándar abierto: el **mismo archivo** corre también en Cursor y Codex CLI.
- Acá es donde llega la versión avanzada: conectar una API de tarifas o búsqueda web estructurada para que los módulos 1 a 4 dejen de estimar y verifiquen de verdad ([roadmap](roadmap.md)).

**Ejemplo:** lo integra en un agente que monitorea una ruta durante semanas y le avisa cuando el precio baja de cierto umbral. El skill deja de ser "consulta puntual" y pasa a "vigilancia automática".

---

## Cómo se conecta con el negocio

Cada nivel es un escalón del mismo embudo:

- **Nivel 1 y 2** → alcance masivo (la gente lo usa gratis donde ya está).
- **Nivel 3** → demostración de que con Claude la cosa se vuelve "mágica" (sin copiar prompts).
- **Nivel 4** → el activo premium / la prueba de que sabés construir, no solo usar.

Un mismo reel puede mostrar los 4 niveles: "lo podés usar gratis en ChatGPT así, o que sea automático en Claude así". Eso te diferencia del resto que solo regala prompts sueltos.

### El embudo de distribución

Reel (comentar palabra) → automatización de ManyChat → sitio web con la guía extendida → link a este repositorio para descargar el skill. La documentación vive en los dos lados: la guía orientada a marketing en el sitio, y la documentación técnica autosuficiente acá en el repo.
