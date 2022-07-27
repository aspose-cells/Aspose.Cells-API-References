---
title: Style
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa el estilo de visualización del documento de Excel como fuente color alineación borde etc. El objeto Estilo contiene todos los atributos de estilo fuente formato de número alineación etc. como propiedades.
type: docs
weight: 5750
url: /es/net/aspose.cells/style/
---
## Style class

Representa el estilo de visualización del documento de Excel, como fuente, color, alineación, borde, etc. El objeto Estilo contiene todos los atributos de estilo (fuente, formato de número, alineación, etc.) como propiedades.

```csharp
public class Style
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Obtiene y establece el color de fondo con un valor ARGB de 32 bits. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Obtiene o establece el color de fondo de un estilo. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Obtiene y establece el color del tema de fondo. |
| [Borders](../../aspose.cells/style/borders) { get; } | Obtiene el[`BorderCollection`](../bordercollection) del estilo. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Obtiene y establece la cadena de patrón dependiente de la referencia cultural para el formato de número. Si no se ha establecido ningún formato de número para este objeto, se devolverá nulo. Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Representa la cadena de formato de número personalizado de este objeto de estilo. Si el formato de número personalizado no está configurado (por ejemplo, el formato de número está integrado), se devolverá "". |
| [Font](../../aspose.cells/style/font) { get; } | Obtiene un[`Font`](./font) objeto. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Obtiene y establece el color de primer plano con un valor ARGB de 32 bits. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Obtiene o establece el color de primer plano de un estilo. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Obtiene y establece el color del tema de primer plano. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Comprueba si se han establecido bordes para el estilo. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Obtiene o establece el tipo de alineación horizontal del texto de una celda. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Representa el nivel de sangría de la celda o rango. Solo puede ser un número entero de 0 a 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Obtiene la cadena de patrón independiente de la referencia cultural para el formato de número. Si no se ha establecido ningún formato de número para este objeto, se devolverá nulo. Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Indica si el formato de número es un formato de fecha. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Indica si el sombreado de la celda es un patrón de degradado. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Indica si en la última línea de texto se deben utilizar las celdas con alineación justificada o distribuida. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Obtiene o establece un valor que indica si una celda se puede modificar o no. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Indica si el formato de número es un formato de porcentaje. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Obtiene o establece un valor que indica si el texto dentro de una celda está ajustado. |
| [Name](../../aspose.cells/style/name) { get; set; } | Obtiene o establece el nombre del estilo. |
| [Number](../../aspose.cells/style/number) { get; set; } | Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes para diferentes regiones. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Obtiene el estilo padre de este estilo. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Obtiene o establece el tipo de patrón de fondo de la celda. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Indica si el valor de la celda comienza con comillas simples. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Representa el ángulo de rotación del texto. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Representa el orden de lectura del texto. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Obtiene o establece el tipo de alineación vertical del texto de una celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Copia datos de otro objeto de estilo |
| override [Equals](../../aspose.cells/style/equals)(object) | Determina si dos instancias de Estilo son iguales. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Sirve como función hash para un objeto Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Obtenga la configuración de degradado de dos colores. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Comprueba si las propiedades especificadas del estilo se han modificado. Se usa para el estilo de ConditionalFormattings para verificar si las propiedades especificadas de este estilo deben usarse al aplicar ConditionalFormattings en una celda. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Establece los bordes del estilo. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Establece la cadena de formato de número personalizado de una celda. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Establece el color de fondo. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Establece el relleno especificado en un degradado de dos colores. |
| [Update](../../aspose.cells/style/update)() | Aplicar el estilo con nombre a los estilos de las celdas que utilizan este estilo con nombre. Funciona como hacer clic en el botón "Aceptar" después de terminar de modificar el estilo. Solo se aplica al estilo con nombre. |

### Ejemplos

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
