---
title: "TickLabelItem.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabelItem. Ancho del elemento Ticklabel como una proporción del ancho del gráfico"
type: docs
url: /es/net/aspose.cells.charts/ticklabelitem/width/
---
## TickLabelItem.Width property

Ancho del elemento Ticklabel como proporción del ancho del gráfico.

```csharp
public double Width { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyWidthDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular gráfico
            chart.Calculate();

            // Acceder a los elementos de etiqueta de marcas
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Demostrar la propiedad Width añadiendo formas que coincidan con las dimensiones de la etiqueta de marca
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Agregar rectángulo que coincida con las dimensiones de la etiqueta de marca (usando la propiedad Width)
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Guarda el libro de trabajo
            workbook.Save("TickLabelItemWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


