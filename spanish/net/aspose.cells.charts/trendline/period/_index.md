---
title: "Trendline.Period"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Devuelve o establece el período para la línea de tendencia movingaverage"
type: docs
url: /es/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Devuelve o establece el período para la línea de tendencia de media móvil.

```csharp
public int Period { get; set; }
```

### Observaciones

Este valor debe estar entre 2 y 255. Y debe ser menor que el número de puntos del gráfico en la serie

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Agregar una línea de tendencia de media móvil
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Guarda el libro de trabajo
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


