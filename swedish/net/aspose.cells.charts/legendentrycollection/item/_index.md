---
title: "LegendEntryCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LegendEntryCollection-egenskap. Hämtar LegendEntry-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Hämtar [`LegendEntry`](../../legendentry/) elementet på det angivna indexet.

```csharp
public LegendEntry this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Category 2");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Åtkomst till legendposter
            LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Demonstrera användning av Item-egenskapen
            for (int i = 0; i < legendEntries.Count; i++)
            {
                LegendEntry entry = legendEntries[i];
                Console.WriteLine($"Legend Entry {i}:");
                Console.WriteLine($"- Font: {entry.Font.Name}");
                Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
            }

            // Ändra första förklaringsposten
            if (legendEntries.Count > 0)
            {
                legendEntries[0].Font.Name = "Arial";
                legendEntries[0].Font.Size = 12;
                legendEntries[0].AutoScaleFont = false;
            }
        }
    }
}
```

### Se även

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


