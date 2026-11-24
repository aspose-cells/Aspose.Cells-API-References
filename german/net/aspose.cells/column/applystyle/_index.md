---
title: "Column.ApplyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Methode. Wendet Formate auf eine ganze Spalte an"
type: docs
url: /de/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Wendet Formate für eine ganze Spalte an.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Beispiele

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

            // Mehrzeiligen Text in Spalte 2 festlegen
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Stil mit aktiviertem Textumbruch erstellen
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Stil nur auf die Eigenschaft Textumbruch von Spalte 2 anwenden
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


