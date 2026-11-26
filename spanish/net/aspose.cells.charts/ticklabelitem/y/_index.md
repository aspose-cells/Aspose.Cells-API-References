---
title: "TickLabelItem.Y"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabelItem. Coordenadas Y del elemento Ticklabel como una proporción de la altura del gráfico"
type: docs
url: /es/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Coordenadas Y del elemento Ticklabel como proporción de la altura del gráfico.

```csharp
public double Y { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // Establecer datos del eje de categorías usando NSERIES en lugar de CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Calcular el gráfico para asegurar que se generen las etiquetas de marcas
            chart.Calculate();

            // Obtener los elementos de etiqueta de marcas del eje de categorías
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Demostrar el uso de la propiedad Y añadiendo formas alineadas con las etiquetas de marcas
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Agregar un rectángulo en la posición Y de cada etiqueta de marca
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Guarda el libro de trabajo
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


