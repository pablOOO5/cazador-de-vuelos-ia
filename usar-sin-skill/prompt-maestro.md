# Prompt maestro — Cazador de Vuelos (versión sin instalar nada)

¿No usás Claude Code ni tenés un plan que permita instalar skills? No pasa nada. Este es el **mismo cerebro del skill condensado en un solo prompt** que copiás y pegás en cualquier chat de IA: ChatGPT, Gemini, Copilot o Claude, incluso en sus versiones gratis.

## Cómo usarlo (3 pasos)

1. **Activá la búsqueda web** del modelo. Sin esto, el modelo *estima* en lugar de verificar (en ChatGPT: el botón de buscar/web; en Gemini suele venir activa; en Claude: activá la búsqueda web). Mirá la guía: [`../guias/chatgpt-gemini-claude-free.md`](../guias/chatgpt-gemini-claude-free.md).
2. **Copiá el prompt de abajo** y reemplazá lo que está `[ENTRE CORCHETES]` con tus datos.
3. **Mandalo.** Si querés profundizar después (mail de negociación, análisis de riesgo, hidden city, etc.), pedíselo en lenguaje natural en el mismo chat.

---

## El prompt (copiá y pegá)

```
Sos un cazador de tarifas aéreas experto. Quiero el pasaje más barato y conveniente
posible de [ORIGEN] a [DESTINO], saliendo alrededor del [FECHA TENTATIVA] con
[X DÍAS] de flexibilidad. Presupuesto: [PRESUPUESTO o "lo más barato posible"].
Prioridad: [precio a toda costa / equilibrio precio y tiempo de viaje].

Usá búsqueda web para trabajar con datos reales. Nunca inventes precios, códigos ni
disponibilidad: si no podés confirmar algo hoy, decilo. Marcá siempre qué es dato
verificado (con fuente) y qué es estimación.

Hacé esto y devolvémelo ordenado:
1. Las 3 mejores combinaciones de fecha de ida y vuelta, en tabla, con precio total
   y por qué cada una conviene.
2. Aerolíneas que vuelan esa ruta, incluyendo low cost y regionales que suelen quedar
   afuera de Google Flights o Skyscanner, ordenadas de menor a mayor precio.
3. 1 o 2 rutas con escalas estratégicas que bajen el costo, con el ahorro estimado vs.
   el vuelo directo.
4. Promos o códigos vigentes HOY (solo los que puedas verificar con fuente).
5. Costos ocultos a tener en cuenta (equipaje, asiento, cambios) y cómo evitarlos.

Cerrá con una recomendación final: la opción que elegirías y por qué.
```

---

## Para ir más a fondo (módulos extra)

El prompt de arriba cubre lo esencial (los 5 módulos más usados). Si querés exprimir todo, en el mismo chat pedí cualquiera de estos:

- **Mail de negociación** → "Redactame un correo firme pero cordial a [aerolínea] para que igualen este precio que encontré: [precio/fuente]."
- **Flexibilidad y riesgo** → "Comparame las políticas de cambio, cancelación y reembolso de estas dos opciones y decime cuál es menos riesgosa. Marcá la letra chica." (pegá las dos opciones)
- **Hidden city ticketing** → "Evaluá si un boleto con destino final más allá de [destino] me sale más barato, y explicame los riesgos reales." *(Ojo: puede violar los términos de la aerolínea; es información, no recomendación.)*

> **Límite honesto:** sin búsqueda web activa, el modelo va a estimar. El prompt le exige marcar qué es estimación. Sin web sirve para orientarte; con web, para decidir. Más detalle en [`../guias/regla-de-oro-y-limites.md`](../guias/regla-de-oro-y-limites.md).
