---
title: "Trendline.DisplayRSquared"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Indica si el valor Rsquared de la línea de tendencia se muestra en el gráfico en la misma etiqueta de datos que la ecuación. Establecer esta propiedad en True activa automáticamente las etiquetas de datos"
type: docs
url: /es/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Representa si el valor R-cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos.

```csharp
public bool DisplayRSquared { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Agregar una línea de tendencia y obtenerla por índice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // Demostrar la propiedad DisplayRSquared
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Guarda el libro de trabajo
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


