---
title: "Legend.LegendEntries"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Legend-egenskap. Hämtar en samling av alla LegendEntry-objekt i den angivna diagramlegenden. Att ställa in legendposterna för ytdiagram stöds inte. Så den returnerar null om diagramtypen är ytdiagramtyp."
type: docs
url: /sv/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Hämtar en samling av alla LegendEntry-objekt i den angivna diagramförklaringen. Att ställa in förklaringsposter för ytdiagram stöds inte. Så den returnerar null om diagramtypen är ytdiagram.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Åtkomst till legendposter
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Ta bort den andra legendposten
            legendEntries[1].IsDeleted = true;
            
            // Spara arbetsboken
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Se även

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


