# Instalar el skill en Claude Code (dev / power user)

Si usás **Claude Code** (la CLI de Anthropic), instalás el skill a nivel sistema y queda disponible en todas tus sesiones. Es la versión para quien lo quiere versionar, mejorar y, más adelante, conectar a datos reales.

## Instalación

1. **Descargá el repo** (clon o ZIP):
   ```bash
   git clone https://github.com/<TU-USUARIO>/cazador-de-vuelos-ia.git
   ```
2. **Copiá la carpeta del skill** a tu directorio de skills de Claude Code:

   **macOS / Linux:**
   ```bash
   cp -r cazador-de-vuelos-ia/skill/vuelos-baratos ~/.claude/skills/
   ```

   **Windows (PowerShell):**
   ```powershell
   Copy-Item -Recurse "cazador-de-vuelos-ia\skill\vuelos-baratos" "$env:USERPROFILE\.claude\skills\"
   ```
3. **Abrí una sesión** de Claude Code y verificá que aparezca:
   ```
   /skills
   ```
   Tenés que ver `vuelos-baratos` en la lista.

## Usarlo

En cualquier sesión, hablale en lenguaje natural:

```
encontrame vuelos baratos de Buenos Aires a Madrid en septiembre,
tengo 4 días de flexibilidad y me importa más el precio
```

El skill se activa solo y corre el modo que corresponda (rápido / experto / módulo puntual). Para los módulos que dependen de precios reales (1 a 4), conviene tener una herramienta de búsqueda web habilitada en tu entorno.

## Bonus: el mismo archivo corre en otras herramientas

El formato `SKILL.md` es un estándar abierto. La **misma carpeta** `vuelos-baratos/` funciona también en **Cursor** y **Codex CLI** sin cambios. Copiala al directorio de skills/agents que use cada herramienta.

## Para el que lo quiere llevar más lejos

Acá es donde el skill puede dejar de estimar y empezar a verificar de verdad: conectándolo a una API de tarifas o a búsqueda web estructurada, o integrándolo en un agente que **monitoree una ruta durante semanas** y avise cuando el precio baje de un umbral. Esa visión está en [`../roadmap.md`](../roadmap.md).
