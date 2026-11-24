---
title: "Top10.Rank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10-Eigenschaft. Liest oder setzt den Wert von n in einer Top/Bottom-n-Regel für bedingte Formatierung. Wenn IsPercent true ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Standardwert ist 10"
type: docs
url: /de/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Abrufen oder Festlegen des Werts von „n“ in einer „top/bottom n“-Bedingten‑Formatierungsregel. Wenn IsPercent true ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Standardwert ist 10.

```csharp
public int Rank { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


