---
title: "Clase TickLabelItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.TickLabelItem. Representa una etiqueta de marca en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Representa una etiqueta de marca en el gráfico.

```csharp
public class TickLabelItem
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Altura del elemento Ticklabel como proporción de la altura del gráfico. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Ancho del elemento Ticklabel como proporción del ancho del gráfico. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | Coordenadas X del elemento Ticklabel como proporción del ancho del gráfico. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Coordenadas Y del elemento Ticklabel como proporción de la altura del gráfico. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular gráfico
            chart.Calculate();

            // Acceder a las etiquetas de marca del eje de categorías
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Agregar formas para marcar la posición de cada etiqueta de marca
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Agregar rectángulo alrededor de la etiqueta de marca
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Agregar círculo junto a la etiqueta de marca
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Guarda el libro de trabajo
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


