# Instalar el skill en Claude.ai (plan pago)

Si usás Claude.ai con un plan pago, podés cargar el skill **una sola vez** y después, en cualquier chat, escribir tu pedido en lenguaje natural. No copiás prompts nunca más: le hablás y resuelve.

## Qué vas a necesitar

- Una cuenta de Claude.ai con un **plan que permita skills** (los skills están en planes pagos).
- La carpeta del skill: `skill/vuelos-baratos/` de este repo (contiene `SKILL.md`).

## Descargar el skill

1. Descargá este repositorio (botón **Code → Download ZIP** en GitHub, o cloná con git).
2. Descomprimí y ubicá la carpeta `skill/vuelos-baratos/`. Esa es la que vas a subir.

## Cargar el skill en Claude.ai

1. En Claude.ai, abrí **Configuración / Settings**.
2. Entrá a la sección de **Skills / Capabilities**.
3. Elegí **agregar / subir un skill** y seleccioná la carpeta `vuelos-baratos/` (la que tiene el `SKILL.md` adentro).
4. Confirmá. El skill queda disponible en tu cuenta.

> La ubicación exacta del menú de skills puede variar según la versión de Claude.ai. Buscá "Skills" dentro de Configuración.

## Usarlo

En cualquier chat nuevo, escribí tu pedido en lenguaje natural. El skill se activa solo:

- *"Encontrame vuelos baratos de Buenos Aires a Madrid en septiembre, tengo 4 días de flexibilidad y me importa más el precio que el tiempo."*
- *"Redactame el mail de negociación para esta aerolínea."*
- *"Comparame el riesgo de estas dos opciones de vuelo."* (pegá las dos)

Claude corre el pipeline que corresponda sin que tengas que saber que detrás hay 8 módulos.

> **Activá la búsqueda web** del chat para que verifique precios reales. Sin web, va a estimar y lo va a aclarar (Regla de oro). Ver [`regla-de-oro-y-limites.md`](regla-de-oro-y-limites.md).

## ¿Y en Claude Cowork?

Si usás Claude Cowork, el skill queda disponible como una capacidad del agente: podés pedirle que arme la búsqueda de vuelos mientras trabaja en otra cosa (por ejemplo, planificando un viaje de negocios completo).
