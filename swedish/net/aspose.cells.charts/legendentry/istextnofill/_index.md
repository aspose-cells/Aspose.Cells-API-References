---
title: "LegendEntry.IsTextNoFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LegendEntry egenskap. Hämtar eller anger ingen fyllning av texten"
type: docs
url: /sv/net/aspose.cells.charts/legendentry/istextnofill/
---
## LegendEntry.IsTextNoFill property

Hämtar eller anger ingen fyllning av texten.

```csharp
public bool IsTextNoFill { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsTextNoFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Åtkomst till legendposten och ange IsTextNoFill
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.IsTextNoFill = true; // Text will have no fill
            
            // Spara arbetsboken
            workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


