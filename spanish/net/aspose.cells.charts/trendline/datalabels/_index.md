---
title: "Trendline.DataLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Representa el objeto DataLabels para la serie especificada"
type: docs
url: /es/net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Representa el objeto DataLabels para la serie especificada.

```csharp
public DataLabels DataLabels { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDataLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Agregar serie y establecer línea de tendencia
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");

            // Configurar DataLabels para la línea de tendencia
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Red;
            trendline.DataLabels.Font.IsBold = true;
            trendline.DataLabels.Position = LabelPositionType.Above;
            trendline.DataLabels.Border.IsVisible = true;
            trendline.DataLabels.Border.Color = Color.Black;

            // Guarda el libro de trabajo
            workbook.Save("TrendlineDataLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


