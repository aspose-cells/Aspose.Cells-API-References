---
title: "Series.Overlap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Anger hur staplar och kolumner placeras. Kan vara ett värde mellan 100 och 100. Gäller endast 2D stapeldiagram och 2D kolumndiagram."
type: docs
url: /sv/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Anger hur staplar och kolumner placeras. Kan vara ett värde mellan -100 och 100. Gäller endast 2‑D stapeldiagram och 2‑D kolumndiagram.

```csharp
public short Overlap { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Lägg till ett grupperat kolumndiagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in överlappningsegenskapen för den första serien
            chart.NSeries[0].Overlap = -40;

            // Spara arbetsboken
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


