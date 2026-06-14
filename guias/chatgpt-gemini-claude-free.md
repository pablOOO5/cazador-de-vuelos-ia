# Usarlo en ChatGPT, Gemini o Claude (incluso gratis)

Esta es la puerta de entrada más fácil: **no instalás nada**. Copiás un prompt, activás la búsqueda web y listo. Funciona en las versiones gratis de los principales modelos.

## El paso que no te podés saltar: activar la búsqueda web

El Cazador de Vuelos vive o muere por una regla: **nunca inventar precios**. Para que el modelo verifique de verdad en vez de estimar, necesita acceso a internet. Activalo así:

| Herramienta | Cómo activar la búsqueda web |
|---|---|
| **ChatGPT** (free y pago) | Tocá el ícono de **buscar en la web** (la lupa/globo) en la barra del mensaje, o escribí "buscá en la web" dentro del prompt. |
| **Gemini** | Suele venir activa por defecto (Google integra búsqueda). Si dudás, pedile "verificá con búsqueda actual". |
| **Claude** (claude.ai) | Activá la **búsqueda web** desde el menú de herramientas del chat. En la app gratis puede estar limitada: si no la ves, el modelo va a estimar (y lo va a aclarar). |
| **Copilot** (Microsoft) | Trae búsqueda web integrada; está activa por defecto. |

> Si la herramienta **no** tiene búsqueda web disponible, el prompt igual sirve para orientarte: le pedimos que marque cada número como **estimación**. Pero para decidir una compra, usá una herramienta con web.

## Pasos

1. **Abrí** ChatGPT, Gemini, Claude o Copilot.
2. **Activá la búsqueda web** (tabla de arriba).
3. **Copiá el prompt maestro** desde [`../usar-sin-skill/prompt-maestro.md`](../usar-sin-skill/prompt-maestro.md).
4. **Reemplazá los `[CORCHETES]`** con tu origen, destino, fechas, flexibilidad y presupuesto.
5. **Mandá.** Revisá que la respuesta marque qué es dato verificado (con fuente) y qué es estimación.
6. **Profundizá** pidiendo en el mismo chat los módulos extra (mail de negociación, riesgo, hidden city).

## Tip

Si querés ir módulo por módulo en vez de todo de una, podés pegar pedidos sueltos: "¿qué aerolíneas low cost vuelan de Buenos Aires a Lima?" o "redactame el mail de negociación". El modelo no necesita el prompt completo para una sola etapa.

## ¿Querés que sea automático?

Si usás Claude, podés instalar el skill y olvidarte de copiar prompts: le hablás en lenguaje natural y resuelve solo.
- En Claude.ai (plan pago): [`claude-ai-skill.md`](claude-ai-skill.md)
- En Claude Code (dev): [`claude-code-skill.md`](claude-code-skill.md)
