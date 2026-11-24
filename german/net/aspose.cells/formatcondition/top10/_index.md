---
title: "FormatCondition.Top10"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Gibt die Top10-Instanz der bedingten Formatierungen zurück. Die Standardregel hebt Zellen hervor, deren Werte in die Top‑10‑Kategorie fallen. Gültig nur, wenn der Typ Top10 ist."
type: docs
url: /de/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Rufen Sie die "Top10"-Instanz der bedingten Formatierung ab. Die Regel der Standardinstanz hebt Zellen hervor, deren Werte in die Top‑10‑Kategorie fallen. Gültig nur für Typ = Top10.

```csharp
public Top10 Top10 { get; }
```

### Beispiele

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

### Siehe auch

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


