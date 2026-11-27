---
title: "Sparkline.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Sparkline‑egenskap. Hämtar radindexet för sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Hämtar radindex för sparkline.

```csharp
public int Row { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Lägg till sparkline på rad 0, kolumn 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Visa radposition (skrivskyddad egenskap)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // För att ändra positionen måste vi ta bort och återskapa sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Spara arbetsbok
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


