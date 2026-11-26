---
title: "Clase Legend"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.Legend class. Encapsula el objeto que representa la leyenda del gráfico"
type: docs
url: /es/net/aspose.cells.charts/legend/
---
## Legend class

Encapsula el objeto que representa la leyenda del gráfico.

```csharp
public class Legend : ChartTextFrame
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Obtiene el [`area`](../chartframe/area/).(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.(Heredado de [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.(Heredado de [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Obtiene el [`border`](../../aspose.cells.drawing/line/).(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Representa la altura de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Representa el ancho de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Representa x de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Representa x de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Representa y de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | Obtiene y establece la dirección del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | Obtiene un objeto [`Font`](../chartframe/font/) del objeto ChartFrame especificado.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsoleto.**) Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Obtiene o establece la altura del marco en unidades de píxeles.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Obtiene o establece la altura del marco en unidades de la proporción del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indica si el texto del gráfico se rota automáticamente.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indica si el marco del gráfico tiene tamaño automático.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | Indica que el texto se genera automáticamente.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indica si esta etiqueta de datos está eliminada.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay/) { get; set; } | Obtiene o establece si se muestra la leyenda sin superponerse al gráfico. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático ocurre cuando el texto dentro de una forma se escala para contener todo el texto dentro.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Obtiene o establece un valor que indica si el texto está ajustado.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries/) { get; } | Obtiene una colección de todos los objetos LegendEntry en la leyenda del gráfico especificado. No se admite establecer las entradas de leyenda del gráfico de superficie. Por lo tanto, devolverá null si el tipo de gráfico es de superficie. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels/) { get; } | (**Obsolete.**) Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Obtiene y establece una referencia a la hoja de cálculo.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [Position](../../aspose.cells.charts/legend/position/) { get; set; } | Obtiene o establece el tipo de posición de la leyenda. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Representa el orden de lectura del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Representa el ángulo de rotación del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True si el marco tiene sombra.(Hereda de [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Obtiene el objeto [`ShapeProperties`](../chartframe/shapeproperties/).(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [Text](../../aspose.cells.charts/charttextframe/text/) { get; set; } | Obtiene o establece el texto del título de un marco.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsoleto.**) Representa el orden de lectura del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsoleto.**) Obtiene un objeto [`Font`](../chartframe/font/) del objeto ChartFrame especificado.(Hereda de [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Obtiene y establece la alineación horizontal del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Obtiene y establece las opciones del texto.(Hereda de [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Obtiene o establece la alineación vertical del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsoleto.**) Obtiene o establece el ancho del marco en unidades de 1/4000 del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Obtiene o establece el ancho del marco en unidades de píxel.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Obtiene o establece el ancho del marco en unidades de proporción del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de píxel.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de píxeles.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de proporción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [GetLegendLabels](../../aspose.cells.charts/legend/getlegendlabels/)() | Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate(). |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Establece la posición del marco a automática(Hereda de [`ChartFrame`](../chartframe/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class LegendDemo
    {
        public static void LegendExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Obtener la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accede a la leyenda del gráfico
            Legend legend = chart.Legend;

            // Establecer propiedades de la leyenda
            legend.Position = LegendPositionType.Left;
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;
            legend.IsOverLay = false;
            legend.IsAutoText = true;
            legend.IsDeleted = false;
            legend.TextHorizontalAlignment = TextAlignmentType.Center;
            legend.TextVerticalAlignment = TextAlignmentType.Center;
            legend.RotationAngle = 0;
            legend.Text = "Legend Text";
            legend.LinkedSource = "Sheet1!A1";
            legend.TextDirection = TextDirectionType.LeftToRight;
            legend.ReadingOrder = TextDirectionType.Context;
            legend.DirectionType = ChartTextDirectionType.Horizontal;
            legend.IsTextWrapped = true;
            legend.IsResizeShapeToFitText = true;
            legend.IsInnerMode = false;
            legend.AutoScaleFont = true;
            legend.BackgroundMode = BackgroundMode.Transparent;
            legend.IsAutomaticSize = true;
            legend.X = 100;
            legend.Y = 100;
            legend.Height = 200;
            legend.Width = 200;
            legend.Shadow = true;

            // Guarda el libro de trabajo
            workbook.Save("LegendExample.xlsx");
            workbook.Save("LegendExample.pdf");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


