---
title: "ErrorBar.Amount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Representerar mängden för felstapeln"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/amount/
---
## ErrorBar.Amount property

Representerar mängden felstapel.

```csharp
public double Amount { get; set; }
```

### Anmärkningar

Mängden måste vara större än eller lika med noll.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyAmountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera felstaplar
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5; // Demonstrate Amount property
            }

            workbook.Save("ErrorBarAmountDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


