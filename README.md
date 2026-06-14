# 🛫 Cazador de Vuelos

> Un cazador de tarifas aéreas experto, dentro de tu IA. Encontrá el pasaje más barato y conveniente mirando lo que el viajero promedio no ve: aerolíneas ocultas, escalas estratégicas, costos escondidos y letra chica.

Esto es la evolución de aquel carrusel viral de prompts para encontrar vuelos baratos con IA: lo mismo, pero **estructurado, con comandos claros y listo para usar en la herramienta que ya tenés** — incluso gratis.

---

## ⚡ Empezá en 3 pasos (lo más rápido)

1. Abrí **ChatGPT, Gemini o Claude** y **activá la búsqueda web**.
2. Copiá el [**prompt maestro**](usar-sin-skill/prompt-maestro.md) y completá tus datos (origen, destino, fechas).
3. Mandalo. Vas a recibir las mejores fechas, aerolíneas ocultas, escalas que ahorran, promos vigentes y costos escondidos.

¿Querés que sea automático y no copiar nada? Instalá el skill 👇

---

## 🎯 Elegí tu herramienta

| Si vos… | Usá esto | Guía |
|---|---|---|
| Usás un chat de IA y no querés instalar nada (incluso gratis) | El **prompt maestro** (copiar y pegar) | [Guía ChatGPT/Gemini/Claude](guias/chatgpt-gemini-claude-free.md) |
| Usás **Claude.ai** (plan pago) y querés que sea automático | El **skill** cargado | [Guía Claude.ai](guias/claude-ai-skill.md) |
| Sos dev / power user y usás **Claude Code** (o Cursor, Codex) | El **skill** instalado a nivel sistema | [Guía Claude Code](guias/claude-code-skill.md) |

Es **el mismo cerebro** en los tres casos. Cambia el envase, no el contenido.

---

## 🧭 La regla de oro

**Nunca inventa precios ni códigos.** Verifica con búsqueda web cuando puede, y marca siempre qué es dato confirmado y qué es estimación. Preferimos un "no lo puedo confirmar" honesto antes que una cifra falsa. Por qué esto importa y qué esperar con/sin web: [regla de oro y límites](guias/regla-de-oro-y-limites.md).

---

## 📦 Qué hay en este repo

```
cazador-de-vuelos-ia/
├── skill/vuelos-baratos/SKILL.md   → el skill (la fuente de verdad)
├── usar-sin-skill/prompt-maestro.md → el mismo cerebro como 1 prompt copy-paste
├── guias/                           → cómo usarlo en cada herramienta
│   ├── chatgpt-gemini-claude-free.md
│   ├── claude-ai-skill.md
│   ├── claude-code-skill.md
│   └── regla-de-oro-y-limites.md
├── roadmap.md                       → hacia dónde va (app, datos reales, alertas)
└── plan-transversal-cazador-vuelos.md → la estrategia detrás del producto
```

## 🛠️ Qué hace el skill

Ocho módulos que podés correr todos o de a uno, según lo que pidas:

1. **Fechas óptimas** de salida y regreso
2. **Aerolíneas** que no aparecen en buscadores grandes
3. **Escalas estratégicas** que bajan el costo
4. **Promos y códigos** vigentes (verificados)
5. **Costos ocultos** y cómo evitarlos
6. **Email para negociar** precio con la aerolínea
7. **Flexibilidad y riesgo** (la letra chica)
8. **Hidden city ticketing** (con sus riesgos)

Le hablás en lenguaje natural y corre el modo que corresponda: rápido (lo esencial), experto (todo) o un módulo puntual.

---

## 🗺️ A futuro

App web, conexión a APIs de tarifas reales y monitoreo de precios con alertas. Ver el [roadmap](roadmap.md).

## 📄 Licencia

[MIT](LICENSE) — usalo, modificalo y compartilo libremente.
