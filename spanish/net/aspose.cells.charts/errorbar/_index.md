---
title: "Clase ErrorBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ErrorBar class. Representa la barra de error de la serie de datos"
type: docs
url: /es/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Representa la barra de error de la serie de datos.

```csharp
public class ErrorBar : Line
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Representa la cantidad de la barra de error. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Especifica la longitud de la punta de flecha para el inicio de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Especifica el ancho de la punta de flecha para el inicio de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Especifica una punta de flecha para el inicio de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Especifica los extremos finales.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Representa el color de la línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Especifica el tipo de línea compuesta(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Especifica el tipo de línea de guiones(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Representa el tipo de visualización de la barra de error. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Especifica la longitud de la punta de flecha para el final de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Especifica el ancho de la punta de flecha para el final de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Especifica una punta de flecha para el final de una línea.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Obtiene o establece el tipo de formato.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Representa el relleno degradado.(Her​edado de [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indica si este estilo de línea se asigna automáticamente.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indica si el color de la línea se asigna automáticamente.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Representa si la línea es visible.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Especifica los extremos de unión.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Indica si se formatean las barras de error con una T en la parte superior. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Representa el estilo de la línea.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Obtiene y establece el color del tema.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro).(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Representa el tipo de cantidad de la barra de error. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Obtiene o establece el [`WeightType`](../../aspose.cells.drawing/weighttype/) de la línea.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Obtiene o establece el grosor de la línea en unidades de puntos.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Obtiene o establece el grosor de la línea en unidades de píxeles.(Heredado de [`Line`](../../aspose.cells.drawing/line/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDemo
    {
        public static void ErrorBarExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Agregar datos de muestra a las celdas
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);
            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Agregar NSeries (fuente de datos del gráfico) al gráfico
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configurar barras de error para cada serie en el gráfico
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Propiedades adicionales para demostración
                series.YErrorBar.ShowMarkerTTop = true;
                series.YErrorBar.PlusValue = "=Sheet1!A1";
                series.YErrorBar.MinusValue = "=Sheet1!A2";
                series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
                series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
                series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
                series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
                series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
                series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
                series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
                series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
                series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
                series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
                series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
                series.YErrorBar.Color = System.Drawing.Color.Red;
                series.YErrorBar.Transparency = 0.5;
                series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
                series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
                series.YErrorBar.WeightPt = 2.0;
                series.YErrorBar.WeightPx = 3.0;
                series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
                series.YErrorBar.IsVisible = true;
                series.YErrorBar.IsAuto = false;
            }

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarExample.xlsx");
            workbook.Save("ErrorBarExample.pdf");
        }
    }
}
```

### Ver también

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


