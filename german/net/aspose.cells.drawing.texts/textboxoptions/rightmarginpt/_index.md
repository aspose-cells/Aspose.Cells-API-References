---
title: "TextBoxOptions.RightMarginPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt den rechten Rand zurück und legt ihn in der Einheit Punkte fest."
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Ermittelt und legt den rechten Rand in der Einheit Punkte fest.

```csharp
public double RightMarginPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Setze den rechten Rand in Punkten
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


