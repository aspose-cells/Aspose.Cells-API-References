---
title: "Font.IsNormalizeHeights"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt an, ob die Normalisierung der Höhe auf den Textlauf angewendet werden soll."
type: docs
url: /de/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Gibt an, ob die Höhennormalisierung auf den Textlauf angewendet werden soll.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### Hinweise

Nur für die Schriftarten von Formen oder Diagrammen. HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) Eigenschaft. Diese Eigenschaft wird 12 Monate später seit Januar 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // Setze die IsNormalizeHeights-Eigenschaft.
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // Überprüfen Sie die Eigenschaft
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // Ändere die Eigenschaft.
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


