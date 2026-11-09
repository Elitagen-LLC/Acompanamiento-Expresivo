# Elitagen Agent

Plugin de marca para [Google Antigravity](https://antigravity.google) de
**Elitagen** y el ecosistema psicosocial **Funvepsiarte | Elitagen**:
innovación multidisciplinaria en ciencias de la salud y de la vida.

**Expert Minds. Intelligent Innovation. - THINK. BUILD. EVOLVE.**

## Contenido

### Agentes (`/agents`)

| Agente | Rol |
| --- | --- |
| `elitagen-expert` | Orquestador principal. Innovación en ciencias de la vida a través de los tres verticales de Elitagen (gobernanza de datos e IA, producción científico-creativa, PMO de tecnología sanitaria). Delega el trabajo psicosocial/expresivo en los especialistas siguientes. |
| `facilitador-expresivo` | Facilitador de terapia expresiva Funvepsiarte: diseño paso a paso de sesiones, talleres y ciclos, audio-a-metodología, registros de campo SMAPS. |
| `arquitecto-smaps` | Intervenciones psicosociales comunitarias sobre la pirámide IASC/MHPSS (SMAPS), con el resumen del manual OIM como fuente. |
| `revisor-etico` | Revisión ética y claridad de rol: facilitación/bienestar vs. psicoterapia clínica regulada; consentimientos, avisos éticos, protocolos de derivación. |

### Skills (`/<nombre-de-skill>`)

| Skill | Qué hace |
| --- | --- |
| `facilitacion-expresiva` | Protocolo completo del Gem: menú de bienvenida, recolección de una pregunta por vez, validación de entradas, diseño de sesión en 10 secciones, generación de documentos. Referencia: `references/registros-clinicos-campo.md`. |
| `smaps-intervencion` | Arquitectura de intervenciones SMAPS: enrutado por perfil, reglas de caso activo, diseño en 6 bloques, matriz de 12 puntos. Referencia: `references/resumen-smaps-oim.md` (resumen OIM 2021). |
| `limites-eticos` | Revisión ética de textos/audios/materiales; clasificación de riesgo; redacción de documentos éticos. |
| `expediente-intervencion` | **Pipeline compuesto nuevo**: diseño + revisión ética + documentos operativos + indicadores de monitoreo en un solo expediente - el entregable integral que encadena las tres skills anteriores. |
| `brand-kit` | Paleta oficial, uso de logos, tipografía, disciplina de tagline, cierre corporativo Funvepsiarte, regla de español sin anglicismos. |

### Regla

`rules/AGENTS.md` (siempre activa): voz de marca, disciplina multilingüe y
guardarraíles de cumplimiento y ética - HIPAA, GDPR, HITECH, CCPA/CPRA,
ISO/IEC 27001, Ley de IA de la UE, NIST AI RMF, ISO/IEC 42001, OCDE; sin
citas fabricadas; la facilitación nunca se presenta como psicoterapia
clínica.

## Probar localmente

```bash
agy plugin validate --strict ./elitagen-agent
agy plugin install ./elitagen-agent

# luego en el chat:
/agents                    # elige elitagen-expert, facilitador-expresivo, ...
/facilitacion-expresiva    # o entra directo a una skill
/expediente-intervencion   # pipeline de intervención documentada completa
```

O copia esta carpeta a `~/.gemini/config/plugins/elitagen-agent/` y reinicia
la app.

## Hoja de ruta

- **Servidor MCP** (`mcp_config.json`) - búsqueda de literatura, tracker de
  proyectos, CDN de activos de marca.
- **Hooks de ciclo de vida** (`hooks.json`) - p. ej. un hook `Stop` que fuerce
  la revisión ética (`limites-eticos`) antes de entregar documentos
  terapéuticos.
- **Más Gems** - los asistentes de referencia restantes se pueden portar como
  skills/subagentes adicionales con el mismo patrón.

## Requisitos

- App o CLI de Antigravity (`agy`)
- Sin claves de API, sin acceso a red, sin servicios externos
