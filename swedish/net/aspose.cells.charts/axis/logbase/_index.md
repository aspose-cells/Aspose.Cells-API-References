---
title: "Axis.LogBase"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis property. Representerar den logaritmiska basen. Standardvärdet är 10"
type: docs
url: /sv/net/aspose.cells.charts/axis/logbase/
---
## Axis.LogBase property

Anger den logaritmiska basen. Standardvärdet är 10.

```csharp
public double LogBase { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyLogBaseDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
                worksheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            chart.NSeries.Add($"B2:B10", true);
            chart.NSeries[0].XValues = $"A2:A10";
            chart.NSeries[0].Name = "Logarithmic Series";

            // Konfigurera logaritmisk axel
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
            chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyLogBaseDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


