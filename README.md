# Acompañamiento Expresivo

Asistente de [Google Antigravity](https://antigravity.google) para
facilitación terapéutica expresiva, intervenciones psicosociales y revisión
ética profesional. Desarrollado sobre la metodología de
**[Funvepsiarte](https://funvepsiarte.org/)**, fundación sin fines de lucro
que integra psicología, artes, estética, creatividad y terapias expresivas.

**Arte, estética y creatividad para la expresión.**

Desarrollado por [Elitagen](https://www.elitagen.com/) en alianza con
[Funvepsiarte](https://funvepsiarte.org/).

## Qué hace por ti

Si eres facilitador, terapeuta, coach expresivo, educador, cuidador o
profesional del bienestar, este asistente te ahorra horas de planificación y
te ayuda a trabajar con coherencia metodológica y límites éticos claros:

1. **Diseña sesiones, talleres y ciclos expresivos** - arteterapia, escritura
   terapéutica, movimiento expresivo, dinámicas simbólicas. Te pregunta paso
   a paso y entrega la estructura completa: objetivo, apertura, actividad,
   reflexión, cierre y adaptaciones.
2. **Estructura tus ideas habladas** - convierte audios y transcripciones en
   metodologías claras, planes de sesión, guiones y bitácoras.
3. **Diseña intervenciones psicosociales** - programas comunitarios sobre la
   pirámide SMAPS/MHPSS del IASC, fundamentados en el manual OIM, con
   indicadores, salvaguardas y criterios de derivación.
4. **Cuida tu ética profesional** - revisa tus textos, flyers, webs y audios
   para que la facilitación nunca se confunda con psicoterapia clínica;
   clasifica el riesgo y redacta consentimientos, avisos éticos y protocolos
   de derivación.
5. **Entrega expedientes completos** - diseño + revisión ética + documentos
   operativos + plan de monitoreo en un solo documento, listo para presentar.

## Agentes (`/agents`)

| Agente | Rol |
| --- | --- |
| `coordinador-expresivo` | Agente principal. Entiende tu necesidad, resuelve o delega en los especialistas. |
| `facilitador-expresivo` | Diseño paso a paso de sesiones, talleres y ciclos de terapia expresiva; audio-a-metodología; registros de campo SMAPS. |
| `arquitecto-smaps` | Intervenciones psicosociales comunitarias sobre la pirámide IASC/MHPSS (SMAPS), con el resumen del manual OIM como fuente. |
| `revisor-etico` | Revisión ética y claridad de rol: facilitación/bienestar vs. psicoterapia clínica regulada; documentos éticos. |

## Skills (`/<nombre>`)

| Skill | Qué hace |
| --- | --- |
| `facilitacion-expresiva` | Menú de bienvenida, recolección de una pregunta por vez, validación de entradas, diseño en 10 secciones, generación de documentos. Referencia: `references/registros-clinicos-campo.md`. |
| `smaps-intervencion` | Enrutado por perfil, reglas de caso activo, diseño en 6 bloques, matriz de 12 puntos. Referencia: `references/resumen-smaps-oim.md` (resumen OIM 2021). |
| `limites-eticos` | Revisión ética de textos/audios/materiales; clasificación de riesgo; documentos éticos. |
| `expediente-intervencion` | Pipeline compuesto: diseño + ética + documentos operativos + indicadores de monitoreo en un solo expediente. |
| `brand-kit` | Identidad visual Funvepsiarte | Elitagen, cierre corporativo, español sin anglicismos. |

## Probar localmente

```bash
agy plugin validate --strict ./acompanamiento-expresivo
agy plugin install ./acompanamiento-expresivo

# luego en el chat:
/agents                    # elige coordinador-expresivo o un especialista
/facilitacion-expresiva    # o entra directo a una skill
/expediente-intervencion   # expediente completo
```

O copia esta carpeta a `~/.gemini/config/plugins/acompanamiento-expresivo/` y reinicia la
app.

## Requisitos

- App o CLI de Antigravity (`agy`)
- Sin claves de API, sin acceso a red, sin servicios externos
