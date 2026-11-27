---
title: "FormatCondition.Top10"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämta den villkorliga formateringens Top10‑instans. Standardinstansens regel markerar celler vars värden ligger i de 10 bästa. Giltig endast för typen Top10."
type: docs
url: /sv/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Hämta den villkorliga formateringens "Top10"-instans. Standardinstansens regel markerar celler vars värden faller inom de 10 bästa. Giltig endast för typ = Top10.

```csharp
public Top10 Top10 { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
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
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### Se även

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


