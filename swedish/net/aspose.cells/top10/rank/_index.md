---
title: "Top10.Rank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10-egenskap. Hämta eller ange värdet på n i en top/bottom n-regel för villkorsstyrd formatering. Om IsPercent är true måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10"
type: docs
url: /sv/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Hämta eller ange värdet på \"n\" i en \"top/bottom n\"‑villkorsformateringsregel. Om IsPercent är sant måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10.

```csharp
public int Rank { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### Se även

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


