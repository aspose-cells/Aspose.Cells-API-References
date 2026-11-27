---
title: "Column.ApplyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-metod. Tillämpar format för en hel kolumn."
type: docs
url: /sv/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Tillämpar format för en hel kolumn.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in flerradig text i kolumn 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Skapa stil med radbrytning aktiverad
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Applicera stil endast på radbrytnings-egenskapen för kolumn 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


