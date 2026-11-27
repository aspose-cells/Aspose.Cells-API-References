---
title: "Sparkline.DataRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Sparkline-egenskap. Representerar dataområdet för sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Representerar dataintervallet för sparkline-objektet.

```csharp
public string DataRange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyDataRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(7);
            sheet.Cells["A4"].PutValue(2);
            sheet.Cells["A5"].PutValue(9);

            // Lägg till en sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Få åtkomst till den första sparkline och visa dess dataområde
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
        }
    }
}
```

### Se även

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


