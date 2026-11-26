---
title: "Clase DataLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.DataLabels. Encapsula una colección de todos los objetos DataLabel para la Serie especificada"
type: docs
url: /es/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Encapsula una colección de todos los objetos DataLabel para la Serie especificada.

```csharp
public class DataLabels : ChartTextFrame
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Obtiene el [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.(Heredado de [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.(Heredado de [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Obtiene el [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Representa la altura de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Representa el ancho de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Representa x de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Representa x de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Representa y de la posición predeterminada en unidades de la fracción del área del gráfico.(Heredado de [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Obtiene y establece la dirección del texto. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Obtiene la fuente de los DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsoleto.**) Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Obtiene o establece la altura del marco en unidades de píxeles.(Hereda de [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Obtiene o establece la altura del marco en unidades de la proporción del área del gráfico.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indica si el texto del gráfico se rota automáticamente.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indica si el marco del gráfico tiene tamaño automático.(Hereda de [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Indica que el texto se genera automáticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indica si esta etiqueta de datos está eliminada.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes.(Hereda de [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico de pastel. Nota: esta propiedad solo tiene sentido cuando se genera una imagen de gráfico de pastel. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático ocurre cuando el texto dentro de una forma se escala para contener todo el texto dentro.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Obtiene o establece un valor que indica si el texto está ajustado. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Obtiene y establece una referencia a la hoja de cálculo.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Obtiene y establece el formato numérico incorporado. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Representa la cadena de formato para el objeto DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | True si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Representa la posición de la etiqueta de datos. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Representa el orden de lectura del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Representa el ángulo de rotación del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Obtiene o establece el tipo de separador utilizado para las etiquetas de datos en un gráfico. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Obtiene o establece el valor del separador utilizado para las etiquetas de datos en un gráfico. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True si el marco tiene sombra.(Hereda de [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Obtiene el objeto [`ShapeProperties`](../chartframe/shapeproperties/).(Hereda de [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Obtiene o establece el tipo de forma de la etiqueta de datos. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False oculta el valor de porcentaje. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. True para mostrar el nombre de categoría en las etiquetas de datos de un gráfico. False para ocultarlo. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Indica si se muestra el rango de celdas como etiquetas de datos. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Representa el comportamiento de visualización de la clave de leyenda de la etiqueta de datos de un gráfico especificado. True si la clave de leyenda de la etiqueta de datos es visible. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False lo oculta. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Indica si el nombre de la serie se muestra en las etiquetas de datos de un gráfico. True para mostrar el nombre de la serie. False para ocultarlo. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Representa el comportamiento de visualización de los valores de la etiqueta de datos de un gráfico especificado. True muestra los valores. False los oculta. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Obtiene o establece el texto de la etiqueta de datos. |
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
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Aplica la fuente de las etiquetas de datos a todos los nodos hijos. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.(Hereda de [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Establece la posición del marco a automática(Hereda de [`ChartFrame`](../chartframe/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DataLabelsDemo
    {
        public static void DataLabelsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accede a los DataLabels de la primera serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Establece propiedades de DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


