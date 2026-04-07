# Color System Pro
-AI made tool-

**Herramienta profesional de design tokens con jerarquía inteligente, validación WCAG 2.1 y simulación de daltonismo.**

---

## Qué hace

La mayoría de herramientas de validación de color te dan una escala, una calificación de contraste y después te dejan solo. Color System Pro analiza la paleta de color de tu marca, asigna roles semánticos con razonamiento qué verás explicado, valida accesibilidad contra entornos reales de color y te entrega el sistema listo para producción.

Ningún color de tu paleta queda descartado  — cada uno recibe un rol adecuado o una sugerencia de uso concreta.

---

## Features

### Motor de color OKLCH
Genera escalas perceptualmente uniformes de color (50→950) donde el valor 500 es exáctamente el color puro de marca. Se trata del mismo algoritmo de color que usa Tailwind v3, Radix UI y CSS Color Level 4.

### Jerarquía inteligente con razonamiento
Puede asignar roles primarios y roles de estado evaluando propiedades reales de cada color mediante la etiqueta de texto editable ubicada justo al lado del hex input, tales como: saturación, luminosidad, matiz y contraste. Cada decisión viene con una explicación, no solo te arroja un resultado.

### WCAG 2.1
Validación del contraste entre pares reales de la interfaz. Evalúa texto negro y blanco sobre cada botón y elige el de mayor ratio. Muestra niveles AA, AAA y advertencias contextuales.

### Simulación CVD
Muestra cómo se percibe cada color uen los ojos de una persona con deuteranopia, protanopia o tritanopia.

### Exportación lista para producción
- **CSS Variables** — generados con prefijo y nombres de rol editables
- **JSON Tokens** — compatible con los tokens de Figma, Style Dictionary y Theo
- **Tailwind Config** — escalas completas y objetos semánticos listos para usar

### Extracción de imagen
Puedes subir una imagen o captura de pantalla y la herramienta extraerá los colores usando el motor de color OKLCH.

### Asesoría, no rechazos
Si tu color primario es un color brillante que no pasa contrastes sobre fondos claros en herramientas tradicionales, color system pro no lo descarta del análisis, por el contrario, le asigna una función, te explica el por qué lo asignó a esa función y da consejos de combinación de color para que este resalte de forma armónica. Cada color tiene un lugar en el sistema.

---

## Tecnología implementada

- **Vanilla HTML** — sin frameworks, sin dependencias, con un peso de 90kb, y apto para funcionar offline
- **OKLCH color math** — implementado desde cero sin uso de librerías externas
- **WCAG 2.1** — uso de cálculo de luminancia relativa según especificación de contraste W3C
- **CVD simulation** — matrices de transformación para deuteranopia, protanopia y tritanopia

---

## Uso paso a paso

1. Ingresa el código hex de tu paleta de color, un código hex por espacio
2. O puedes subir una captura de pantalla para extraer colores automáticamente
3. Da click en el botón de Analizar y Generar sistema
4. Edita cualquier asignación con los dropdowns si no te convence la asignación automática o si prefieres mantener un control total sobre las asignaciones. 
5. Exporta en CSS, JSON o Tailwind con tu propia semántica

---

## Roles que puede generar

| Rol | Descripción |
|-----|-------------|
| Clickable | Botón primario, links, CTA |
| Hover / activo | Estado hover y focus |
| Texto principal | Títulos y cuerpo de texto |
| Texto secundario | Labels, hints, subtítulos |
| Fondo de página | Base de la interfaz |
| Fondo de card | Superficies y paneles |
| Resalto / badge | Tags y notificaciones |
| Borde | Separadores y outlines |
| Éxito | Confirmaciones, checks |
| Error | Validaciones fallidas |
| Advertencia | Alertas, precaución |
| Información | Tooltips, banners |
| Neutro / UI | Grises, superficies neutras |
| Decorativo | Ilustraciones, gráficos |

---

## Autor

**MCSangel** — AI Senior Creative Designer · UI Designer · Illustrator

---

*Hecho con amor · 2026*
