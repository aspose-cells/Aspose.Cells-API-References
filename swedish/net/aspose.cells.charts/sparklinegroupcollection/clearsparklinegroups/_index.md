---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroupCollection‑metod. Rensar Sparkline‑grupperna som överlappar ett cellområde"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Rensar sparkline-grupperna som överlappar ett cellområde.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | Anger cellområdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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
                // Anropa ClearSparklineGroups‑metoden med CellArea‑parameter
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Verifiera antalet Sparkline‑grupper efter rensning
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


