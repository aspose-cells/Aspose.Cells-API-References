---
title: "SparklineGroup.LineWeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Hämtar och anger linjetjockleken för varje linjesparkline i sparkline-gruppen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Hämtar och anger linjebredden i varje linjesparkline i sparkline-gruppen, i enheten punkter.

```csharp
public double LineWeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLineWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Skapa sparkline-grupp
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Ställ in LineWeight-egenskap
            group.LineWeight = 2.5; // Thicker line weight for visibility

            workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


