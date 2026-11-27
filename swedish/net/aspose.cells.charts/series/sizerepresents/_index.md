---
title: "Series.SizeRepresents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Hämtar eller anger vad bubbelstorleken representerar i ett bubbel‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Hämtar eller anger vad bubbelstorleken representerar i ett bubbeldiagram.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Anmärkningar

`BubbleSizeRepresents.SizeIsArea` betyder att värdet [`BubbleSizes`](../bubblesizes/) är bubblans area. `BubbleSizeRepresents.SizeIsWidth` betyder att värdet [`BubbleSizes`](../bubblesizes/) är bubblans bredd.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för bubbeldiagram
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Lägg till ett bubbeldiagram
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ange seriedata
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // Ställ in SizeRepresents‑egenskapen
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Spara arbetsboken
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


