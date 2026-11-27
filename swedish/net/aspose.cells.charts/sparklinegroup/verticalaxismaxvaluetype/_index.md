---
title: "SparklineGroup.VerticalAxisMaxValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Representerar den maximala värdetypen för den vertikala axeln"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/
---
## SparklineGroup.VerticalAxisMaxValueType property

Representerar den vertikala axelns maximala värdetyp.

```csharp
public SparklineAxisMinMaxType VerticalAxisMaxValueType { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueTypeDemo
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

            // Definiera sparkline-plats
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Lägg till sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Konfigurera inställningar för vertikal axel
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Spara arbetsboken
            workbook.Save("SparklineVerticalAxisDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


