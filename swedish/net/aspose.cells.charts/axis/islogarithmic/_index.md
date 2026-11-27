---
title: "Axis.IsLogarithmic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger om värdeaxelns skaltyp är logaritmisk eller inte"
type: docs
url: /sv/net/aspose.cells.charts/axis/islogarithmic/
---
## Axis.IsLogarithmic property

Anger om värdeaxelns skaltyp är logaritmisk eller inte.

```csharp
public bool IsLogarithmic { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsLogarithmicDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(1000);
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(100);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries[0].Values = "B1:B4";

            // Konfigurera logaritmisk axel
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 10;
            chart.CategoryAxis.MinValue = 1;
            chart.CategoryAxis.MaxValue = 10000;

            // Spara arbetsboken
            workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


