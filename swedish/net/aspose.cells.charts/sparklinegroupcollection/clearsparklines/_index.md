---
title: "SparklineGroupCollection.ClearSparklines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroupCollection‑metod. Rensar sparkline‑elementen som finns i ett cellområde"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Rensar sparklines som finns inom ett cellområde.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Anger cellområdet |

### Anmärkningar

[`SparklineGroup`](../../sparklinegroup/) will be removed too if it does not contains any [`Sparkline`](../../sparkline/).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            try
            {
                // Anropa ClearSparklines‑metoden med CellArea‑parameter
                sheet.SparklineGroups.ClearSparklines(ca);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


