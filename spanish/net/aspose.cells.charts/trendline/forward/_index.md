---
title: "Trendline.Forward"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Devuelve o establece el número de períodos o unidades en un gráfico de dispersión que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero"
type: docs
url: /es/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero.

```csharp
public double Forward { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Agregar línea de tendencia
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Demostrar la propiedad Forward
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


