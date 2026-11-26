---
title: "TickLabels.TickLabelItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Obtiene las etiquetas de marcas de visualización del eje"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/ticklabelitems/
---
## TickLabels.TickLabelItems property

Obtiene las etiquetas de marcas de visualización del eje.

```csharp
public TickLabelItem[] TickLabelItems { get; }
```

### Observaciones

Solo disponible después de llamar al método [`Calculate`](../../chart/calculate/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTickLabelItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Calcular gráfico
            chart.Calculate();

            // Obtener eje de categoría y sus etiquetas de marcas
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Agregar formas para marcar la posición de cada etiqueta de marca
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Agregar un rectángulo alrededor de cada etiqueta de marca
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;
            }

            // Guarda el libro de trabajo
            workbook.Save("TickLabelItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


