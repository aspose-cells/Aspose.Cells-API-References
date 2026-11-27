---
title: "Sparkline.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Sparkline-egenskap. Hämtar kolumnindexet för sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Hämtar kolumnindexet för sparkline-objektet.

```csharp
public int Column { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Skapa sparkline-grupp
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Lägg till sparkline i kolumn 4 och demonstrera Column-egenskapen
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Visa kolumn-egenskap (skrivskyddad)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // För att ändra kolumnpositionen måste vi ta bort och återlägga sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Spara arbetsbok
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


