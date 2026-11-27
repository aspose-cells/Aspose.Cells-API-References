---
title: "SparklineGroup.ResetRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup metod. Återställer dataområdet och platsområdet för sparkline-gruppen. Denna metod rensar ursprungliga sparkline‑objekt i gruppen och skapar nya sparkline‑objekt för de nya områdena"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Återställer dataintervallet och positionsintervallet för sparkline-gruppen. Denna metod rensar ursprungliga sparkline‑objekt i gruppen och skapar nya sparkline‑objekt för de nya intervallen.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataRange | String | Anger det nya dataområdet för sparkline-gruppen. |
| ärVertikal | Boolean | Anger om sparklines ska plottas från det nya dataområdet radvis eller kolumnvis. |
| locationRange | CellArea | Anger var sparklines ska placeras. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
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

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Förbered parametrar för ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Anropa ResetRanges med parametrarna (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


