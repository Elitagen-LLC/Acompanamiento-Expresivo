---
name: brand-kit
description: >-
  Aplica la identidad visual y la voz de Elitagen a cualquier entregable:
  presentaciones, documentos, páginas web, guiones, one-pagers o
  visualizaciones de datos. Úsala cuando el usuario pida algo "en marca",
  material con marca, un artefacto para clientes, o mencione los
  colores/logos/tagline de Elitagen. Incluye el cierre corporativo
  Funvepsiarte | Elitagen. Se invoca con /brand-kit.
---

# Kit de marca Elitagen

Carga esta skill antes de producir CUALQUIER entregable que un cliente o
aliado de Elitagen pueda ver.

## 1. Paleta de colores (extraída de la marca oficial)

| Rol | Hex | Uso |
| --- | --- | --- |
| Azul marino profundo | `#020345` | Ancla oscuro principal, titulares, lienzos oscuros |
| Azul real | `#0C57A8` | Azul de marca, acentos clave, enlaces |
| Azul acero | `#305090` | Estructura secundaria, bordes, gráficos |
| Cian | `#31A9DC` | Acento de energía, énfasis de datos |
| Cian cielo | `#63C6EB` | Degradados y acentos claros junto al cian |
| Lavanda pálido | `#AEBAEF` | Acento claro, rellenos, fondos sutiles |
| Hielo | `#C0D0F0` | Tinte de fondo suave |
| Blanco | `#FFFFFF` | Espacio negativo, texto sobre oscuro |

Los degradados de la marca se mueven *dentro* de una misma familia (p. ej.
`#63C6EB -> #008CCB`), no entre tonos sin relación. Las interfaces oscuras se
apoyan en azul marino profundo, no en negro puro.

## 2. Logos

- Símbolo incluido: `${PLUGIN_ROOT}/assets/logo.png` - el molinete de cuatro
  lóbulos de Elitagen sobre fondo transparente (1:1). Conserva su margen
  transparente; nunca lo recortes, recolorees, deformes ni lo pongas sobre
  imágenes cargadas.
- Biblioteca completa de logos (lockups, banners, variantes monocromáticas)
  en el repositorio del proyecto, carpeta de mercadeo
  (`06_Logos ... Elitagen_Funvepsiarte`):
  `main_logo.png` (fondos claros), `main_logo_dark.png` (variante sobre fondo
  azul real oscuro), `mono_main_white_logo.png` (monocromo),
  `*_banner_left_*` (lockups anchos), `elitagen_text_blue_font.svg`
  (wordmark).

## 3. Tipografía y maquetación

- Sans-serif geométrica moderna; abundante espacio en blanco, ornamentación
  mínima. (La fuente exacta del sitio no está incluida; usa Inter o Helvetica
  Neue por defecto en activos digitales derivados - confirma con el equipo
  antes de imprimir.)
- Ritmo de secciones del sitio: etiqueta superior -> titular de declaración
  grande -> párrafo breve de apoyo. Bloques de capacidades numerados
  (I, II, III).
- Disciplina de tagline: **"Expert Minds. Intelligent Innovation."** y la
  tríada **THINK. BUILD. EVOLVE.** Nunca alteres la redacción, la traducción
  ni las mayúsculas.

## 4. Lista de voz para entregables

1. Experto y directo - sin exageración, sin adjetivos de relleno.
2. Listo para multilingüe - fraseo idiomático, no traducción literal. En
   español, sin anglicismos.
3. Consciente del cumplimiento - ver `rules/AGENTS.md`; incluye notas de
   revisión cuando el contenido toque temas clínicos o datos de pacientes.
4. Enfoque multidisciplinario - nombra las disciplinas que convergen en cada
   solución.

## 5. Valores por defecto para entregables HTML/Markdown

```css
:root {
  --elitagen-navy: #020345;
  --elitagen-royal: #0C57A8;
  --elitagen-steel: #305090;
  --elitagen-cyan: #31A9DC;
  --elitagen-sky: #63C6EB;
  --elitagen-lavender: #AEBAEF;
  --elitagen-ice: #C0D0F0;
}
```

Titulares: azul marino profundo (o blanco sobre oscuro). Subrayados/botones
de acento: cian. Texto de cuerpo: grises de la familia acero derivados de
`#305090`.

## 6. Cierre corporativo Funvepsiarte | Elitagen

Los asistentes del ecosistema psicosocial (facilitación expresiva, SMAPS,
límites éticos) cierran las interacciones con este bloque centrado:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━
      FUNVEPSIARTE | ELITAGEN
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Gracias por compartir este proceso terapéutico y creativo y por confiar en
este espacio de acompañamiento profesional.

Espero que esta estructura contribuya a crear experiencias:
- claras
- seguras
- emocionalmente significativas

🌐 www.elitagen.com  / 📧 info@elitagen.com
🌐 funvepsiarte.org  / 📧 hola@funvepsiarte.org
```

Variante psicosocial del texto de cierre: "Gracias por compartir este proceso
psicosocial y creativo. Espero que contribuya a experiencias claras, seguras
y significativas."

En español NUNCA uses anglicismos: "aviso ético" o "descargo de
responsabilidad", no "disclaimer".
