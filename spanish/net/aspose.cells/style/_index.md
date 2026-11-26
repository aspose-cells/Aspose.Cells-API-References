---
title: "Clase Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Style class. Representa el estilo de visualización de documentos de Excel, como color de fuente, alineación, borde, etc. El objeto Style contiene todos los atributos de estilo, fuente, formato numérico, alineación y demás como propiedades"
type: docs
url: /es/net/aspose.cells/style/
---
## Style class

Representa el estilo de visualización de un documento Excel, como fuente, color, alineación, borde, etc. El objeto Style contiene todos los atributos de estilo (fuente, formato numérico, alineación, y así sucesivamente) como propiedades.

```csharp
public class Style
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Style](style/)() | (**Obsoleto.**) Inicializa una nueva instancia de la clase `Style`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Obtiene y establece el color de fondo con un valor ARGB de 32 bits. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Obtiene o establece el color de fondo de un estilo. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Obtiene y establece el color del tema de fondo. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Obtiene la [`BorderCollection`](../bordercollection/) del estilo. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Obtiene el borde inferior. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Obtiene y establece la cadena de patrón dependiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Representa la cadena de formato numérico personalizado de este objeto de estilo. Si el formato numérico personalizado no está establecido (Por ejemplo, el formato numérico es incorporado), se devolverá "". |
| [Font](../../aspose.cells/style/font/) { get; } | Obtiene un objeto [`Font`](./font/). |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Obtiene y establece el color de primer plano con un valor ARGB de 32 bits. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Obtiene o establece el color de primer plano de un estilo. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Obtiene y establece el color del tema de primer plano. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Comprueba si se han establecido bordes para el estilo. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Obtiene o establece el tipo de alineación horizontal del texto en una celda. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Representa el nivel de sangría para la celda o el rango. Solo puede ser un entero de 0 a 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Obtiene la cadena de patrón independiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Indica si se debe aplicar el formato de alineación. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Indica si se debe aplicar el formato de borde. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Indica si es un estilo de casilla de verificación. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Indica si el formato numérico es un formato de fecha. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Indica si se debe aplicar el formato de relleno. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Indica si se debe aplicar el formato de fuente. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Indica si el sombreado de la celda es un patrón degradado. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Obtiene o establece un valor que indica si una celda puede modificarse o no. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Indica si se debe aplicar el formato numérico. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Indica si el formato numérico es un formato de porcentaje. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Indica si se debe aplicar el formato de protección. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Obtiene o establece un valor que indica si el texto dentro de una celda está ajustado. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Obtiene el borde izquierdo. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Obtiene o establece el nombre del estilo. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes según la región. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Obtiene el estilo padre de este estilo. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Obtiene o establece el tipo de patrón de fondo de la celda. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Indica si el valor de la celda comienza con una comilla simple. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Obtiene el borde derecho. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Representa el ángulo de rotación del texto. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Representa el orden de lectura del texto. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Obtiene el borde superior. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Obtiene o establece el tipo de alineación vertical del texto en una celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Copia datos de otro objeto de estilo |
| override [Equals](../../aspose.cells/style/equals/)(object) | Determina si dos instancias de Style son iguales. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Sirve como función hash para un objeto Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsoleto.**) Obtiene la configuración de degradado bicolor. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Obtiene la configuración de degradado bicolor. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Comprueba si las propiedades especificadas del estilo han sido modificadas. Se usa para el estilo de ConditionalFormattings para comprobar si las propiedades especificadas de este estilo deben usarse al aplicar ConditionalFormattings en una celda. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Establece los bordes del estilo. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Establece los bordes del estilo. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Establece la cadena de formato numérico personalizado de una celda. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Establece los bordes de contorno |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Establece los bordes de contorno |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Establece el color de fondo. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Establece el relleno especificado a un degradado bicolor. |
| [ToJson](../../aspose.cells/style/tojson/)() | Convierte `Style` a datos estructurados JSON. |
| [Update](../../aspose.cells/style/update/)() | Aplica el estilo nombrado a los estilos de las celdas que usan este estilo nombrado. Funciona como hacer clic en el botón \"ok\" después de haber terminado de modificar el estilo. Solo se aplica al estilo nombrado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a una celda de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            
            // Obtener el estilo de la celda
            Style style = cell.GetStyle();
            
            // Establece varias propiedades del estilo
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Establece el estilo en la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


