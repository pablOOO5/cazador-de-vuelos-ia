# La regla de oro y los límites honestos

Esta es la parte que hace que el Cazador de Vuelos se gane la confianza en vez de quemarla. Leela: entender esto te ahorra frustraciones.

## La regla de oro

> **Nunca inventar precios, códigos, promos, disponibilidad ni rutas concretas.**

Un modelo de IA puede sonar muy seguro y tirar una tabla con números prolijos que **se inventó**. Eso es lo peor que le puede pasar a una herramienta de vuelos: una sola cifra falsa y perdés la confianza. Por eso el skill (y el prompt) tienen instrucciones explícitas para:

- **Verificar con búsqueda web** antes de afirmar cualquier número.
- **Marcar siempre** qué es **dato verificado** (con fuente y fecha) y qué es **estimación**.
- **Descartar** cualquier promo o código que no pueda confirmar vigente hoy.
- Decir **"no lo puedo confirmar"** antes que inventar.

## Con web vs. sin web

| | **Con búsqueda web activa** | **Sin búsqueda web** |
|---|---|---|
| Precios | Verificados, con fuente | Estimados (rango aproximado) |
| Promos/códigos | Solo los confirmados vigentes | No los va a afirmar |
| Para qué sirve | **Decidir** una compra | **Orientarte** sobre qué esperar |

La conclusión práctica: **para decidir, usá una herramienta con búsqueda web.** Cómo activarla en cada una: [`chatgpt-gemini-claude-free.md`](chatgpt-gemini-claude-free.md).

## Lo que el Cazador de Vuelos NO es (todavía)

- **No** es un buscador en tiempo real conectado a las aerolíneas. Trabaja con lo que el modelo puede ver vía búsqueda web en el momento de la consulta.
- **No** compra ni reserva por vos. Te arma la estrategia; la compra la hacés vos en el sitio de la aerolínea o agencia.
- **No** garantiza un precio. Los precios de vuelos cambian todo el tiempo; lo que ves hoy puede no estar mañana.

A futuro, conectándolo a una API de tarifas, los precios pueden pasar de estimados a verificados de punta a punta. Esa es la visión del [`../roadmap.md`](../roadmap.md).

## Sobre el hidden city ticketing (módulo 8)

El módulo de "destinos ocultos" es **información, no recomendación**. El hidden city ticketing puede violar los términos de la aerolínea (riesgo de perder millas, que te cancelen tramos o la cuenta), aunque no es ilegal. El skill te lo explica con sus riesgos para que decidas con todos los datos, no para empujarte a hacerlo.
