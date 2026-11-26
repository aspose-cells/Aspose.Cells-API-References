---
title: "ChartPoint.Explosion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel.

```csharp
public int Explosion { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyExplosionDemo
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

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al primer punto del gráfico y establecer la explosión
            ChartPoint point = chart.NSeries[0].Points[0];
            point.Explosion = 15; // Set explosion distance (15 points)

            // Guarda el libro de trabajo
            workbook.Save("ChartPointExplosionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


