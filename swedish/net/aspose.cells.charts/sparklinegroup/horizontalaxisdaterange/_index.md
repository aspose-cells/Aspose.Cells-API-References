---
title: "SparklineGroup.HorizontalAxisDateRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Representerar intervallet som innehåller datumvärdena för sparkline-data"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/
---
## SparklineGroup.HorizontalAxisDateRange property

Representerar intervallet som innehåller datumvärdena för sparkline‑data.

```csharp
public string HorizontalAxisDateRange { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till datum- och värdedata för sparkline
            sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
            sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
            sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
            
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["D2"].PutValue(3);

            // Definiera CellArea där sparkline kommer att placeras
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 1,
                EndRow = 1
            };

            // Lägg till en sparkline-grupp med datumaxel
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Ställ in datumintervallet för horisontell axel
            group.HorizontalAxisDateRange = "A1:D1";
            group.ShowHorizontalAxis = true;

            // Spara arbetsboken
            workbook.Save("SparklineWithDateAxis.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


