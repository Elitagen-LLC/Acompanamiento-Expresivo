---
name: expediente-intervencion
description: >-
  Produce un expediente COMPLETO de intervención terapéutica expresiva o
  psicosocial en una sola entrega: diseño metodológico + revisión ética +
  documentos operativos (registro/bitácora de campo, consentimiento,
  materiales) + plan de monitoreo e indicadores. Orquesta las skills
  facilitacion-expresiva, smaps-intervencion y limites-eticos. Úsala cuando
  el usuario pida un proyecto documentado, dossier, propuesta para
  financiación o "expediente" de una intervención, no solo un diseño suelto.
  Español por defecto. Se invoca con /expediente-intervencion.

---

# Expediente de Intervencion (pipeline documental completo)

Esta skill compone las tres capacidades Funvepsiarte | Elitagen en un unico
flujo que entrega un expediente reutilizable y auditable. NO improvises pasos
sueltos: sigue el pipeline completo.

## Pipeline (4 fases)

### Fase 1 - Diseño metodologico

- Intervencion terapeutica expresiva (sesion, taller o ciclo): aplica
  `skills/facilitacion-expresiva/SKILL.md` (recoleccion paso a paso de la
  informacion minima y estructura de 10 secciones).
- Intervencion psicosocial comunitaria: aplica
  `skills/smaps-intervencion/SKILL.md` (perfil, fundamentacion por niveles
  SMAPS, matriz rapida de 12 puntos, resumen OIM en
  `skills/smaps-intervencion/references/resumen-smaps-oim.md`).

Entregable de fase: diseño estructurado con objetivo, poblacion, metodologia,
duracion, materiales y pasos.

### Fase 2 - Revision etica del diseño

Pasa el entregable de la Fase 1 por el flujo de
`skills/limites-eticos/SKILL.md`:

1. Detectar lenguaje clinico indebido, promesas de resultados o ambiguedad
   de rol.
2. Clasificar riesgo (Bajo / Medio / Alto).
3. Corregir antes de documentar; registrar las correcciones aplicadas.

Regla: si el riesgo clasifica Alto, NO avances a la Fase 3 hasta corregir.

### Fase 3 - Documentos operativos

Genera los que correspondan al alcance (pregunta cuales necesita el usuario):

- Plan de sesion o guion de facilitacion.
- Registro clinico de campo
  (`skills/facilitacion-expresiva/references/registros-clinicos-campo.md`).
- Bitacora terapeutica o cronograma de implementacion.
- Consentimiento informado, aviso etico y normas de convivencia (lenguaje de
  `limites-eticos`: sin anglicismos, sin promesas clinicas).
- Protocolo de derivacion (rutas de referencia segun nivel SMAPS).

### Fase 4 - Monitoreo e indicadores

Basado en la cadena insumos -> actividades -> productos -> resultados ->
impacto (resumen OIM, seccion 18). Entrega 5-8 indicadores mezclando
cuantitativos y cualitativos: acceso y participacion, percepcion de seguridad
y dignidad, cambios en apoyo social y agencia, fidelidad de facilitacion,
referencias completadas, efectos no deseados. Nunca atribuyas causalidad por
asistencia o satisfaccion.

## Formato del expediente final

Documento unico en Markdown (o el formato que pida el usuario), con este
indice:

1. Portada del expediente (titulo, fecha, responsable, marca Funvepsiarte |
   Elitagen)
2. Resumen ejecutivo (max. 10 lineas)
3. Diseño metodologico (Fase 1)
4. Revision etica: hallazgos, clasificacion y correcciones (Fase 2)
5. Documentos operativos (Fase 3, anexados e integrados)
6. Plan de monitoreo e indicadores (Fase 4)
7. Riesgos, salvaguardas y criterios de referencia
8. Supuestos declarados y pendientes `[NEEDS SME REVIEW]`

## Reglas

- La informacion minima de la fase de diseño se recopila siguiendo el
  protocolo paso a paso de la skill correspondiente (una pregunta por vez en
  facilitacion expresiva; maximo tres breves por tanda en SMAPS). Declara
  supuestos prudentes solo para datos no criticos.
- Inventar datos de poblacion, cifras o resultados esta PROHIBIDO: marca
  `[NEEDS SME REVIEW]`.
- Cualquier contenido clinico (impresion clinica, plan de tratamiento, rutas
  de derivacion) debe marcarse como "requiere validacion de profesional
  competente".
- Idioma: espanol por defecto, sin anglicismos; espejo del idioma del
  usuario. Marca y cierre corporativo segun `skills/brand-kit/SKILL.md`.
