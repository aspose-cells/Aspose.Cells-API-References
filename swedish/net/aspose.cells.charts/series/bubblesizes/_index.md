---
title: "Series.BubbleSizes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar eller anger bubbelstorleksvärdena för diagramserien"
type: docs
url: /sv/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Hämtar eller anger bubbelstorleksvärdena för diagramserien.

```csharp
public string BubbleSizes { get; set; }
```

### Anmärkningar

Endast för Bubble eller Bubble3D.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för bubbeldiagram
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Lägg till ett bubbeldiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ange seriedata med hjälp av egenskapen BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Spara arbetsboken
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


