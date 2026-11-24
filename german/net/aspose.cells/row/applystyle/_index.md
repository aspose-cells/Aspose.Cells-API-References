---
title: "Row.ApplyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Wendet Formate auf eine gesamte Zeile an."
type: docs
url: /de/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Wendet Formate für eine ganze Zeile an.

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
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // HTML‑Inhalt in der ersten Zelle festlegen
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Erhalte die erste Zeile und ihren Stil
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Stileigenschaften ändern
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Stil mit spezifischen Flags anwenden (nur Zeilenumbruch wird angewendet)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Auto‑Fit zur Demonstration
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Speichere die Arbeitsmappe
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


