---
title: "Series.Explosion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel"
type: docs
url: /es/net/aspose.cells.charts/series/explosion/
---
## Series.Explosion property

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
    public class SeriesPropertyExplosionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar gráfico circular
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            int seriesIndex = chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";
            
            // Acceder a la serie y establecer la explosión
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.Explosion = 15; // Set explosion value (0-100)
            
            workbook.Save("PieChartExplosionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


