---
title: "SparklineCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineCollection-metod. Lägg till en sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Lägg till en sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataRange | String | Anger det nya dataintervallet för sparkline. |
| row | Int32 | Radindex för platsen. |
| column | Int32 | Kolumnindex för platsen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Skapa en sparkline-grupp
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Lägg till sparkline med dataintervall och plats
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


