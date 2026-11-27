---
title: "Series.ShowNegativeBubbles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Sant om negativa bubblor visas för diagramgruppen. Gäller endast för bubbeldiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

Sant om negativa bubblor visas för diagramgruppen. Giltigt endast för bubbeldiagram.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för bubbeldiagram
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Lägg till ett bubbeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // Åtkomst till den första serien och ange ShowNegativeBubbles‑egenskapen
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


