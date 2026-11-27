---
title: "SparklineGroup.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger sparkline-typen för sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Anger sparkline-typen för sparkline-gruppen.

```csharp
public SparklineType Type { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
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

            // Skapa sparkline-grupp med kolumntyp
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ändra sparkline-typen till Linje
            group.Type = SparklineType.Line;

            // Lägg till sparkline i gruppen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Spara arbetsboken
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


