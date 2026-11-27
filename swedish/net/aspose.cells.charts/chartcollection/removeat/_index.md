---
title: "ChartCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartCollection-metod. Ta bort ett diagram på det specifika indexet"
type: docs
url: /sv/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Ta bort ett diagram på det specifika indexet.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Diagramindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Visa ursprungligt diagramantal
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // Ta bort diagrammet på index 0
            sheet.Charts.RemoveAt(0);

            // Visa diagramantal efter borttagning
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### Se även

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


