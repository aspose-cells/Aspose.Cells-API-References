---
title: "Top10.IsBottom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10-Eigenschaft. Liest oder setzt, ob eine Top/Bottom-n-Regel eine Bottom-n-Regel ist. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

Abrufen oder Festlegen, ob eine „top/bottom n“-Regel eine „bottom n“-Regel ist. Standardwert ist false.

```csharp
public bool IsBottom { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Bedingte Formatierung hinzufügen
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // Füge Top10-Bedingung hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Konfiguriere Top10-Eigenschaften
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


