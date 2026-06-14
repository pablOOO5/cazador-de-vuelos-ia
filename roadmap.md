# Roadmap — hacia dónde va el Cazador de Vuelos

Hoy el Cazador de Vuelos funciona con la **búsqueda web del propio modelo**: alcanza para orientar y, con web activa, para decidir. Esto es lo que viene si el proyecto crece. Nada de esto está construido todavía; es la visión.

## Etapa actual ✅

- Skill `vuelos-baratos` con 8 módulos y capa de comandos (rápido / experto / módulo puntual).
- Prompt maestro copy-paste para la versión sin instalar nada.
- Documentación para usarlo en ChatGPT/Gemini/Claude, Claude.ai y Claude Code.
- Regla de oro: nunca inventar precios; marcar dato vs. estimación.

## Próximo: datos reales 🔌

El salto de calidad más grande. Conectar los módulos 1 a 4 (los que dependen de precios) a una **API de tarifas** para que dejen de estimar y verifiquen de punta a punta. Candidatas a evaluar:

- **Amadeus Self-Service API** (búsqueda de vuelos y precios).
- **Kiwi / Tequila API** (fuerte en low cost y rutas combinadas, alineado con el módulo de aerolíneas ocultas).
- Agregadores tipo **Skyscanner / Travelpayouts** (afiliación + datos).

Con esto, la tabla de "precio estimado" pasa a "precio verificado con fuente y timestamp".

## Después: monitoreo y alertas 🔔

El skill deja de ser "consulta puntual" y pasa a "vigilancia automática": un agente que **monitorea una ruta durante semanas** y avisa cuando el precio baja de un umbral. Ideal para integrarlo en Claude Code con tareas programadas.

## A futuro: la app 📱

Una **aplicación web** donde quien no usa IA igual pueda cargar origen, destino y fechas, y recibir el análisis completo del Cazador detrás de escena. El skill sería el motor; la app, la cara amigable para el público masivo.

## Distribución 📣

- **Repo público** (este): la fuente de verdad, descargable.
- **Guía extendida en el sitio web**: explicación paso a paso orientada a la audiencia, que linkea a este repo. *(En construcción, se arma aparte.)*
- **Embudo**: reel en redes → automatización → sitio web → repo.

---

¿Ideas o pedidos? Este roadmap es vivo. La prioridad la marca lo que la audiencia más pida.
