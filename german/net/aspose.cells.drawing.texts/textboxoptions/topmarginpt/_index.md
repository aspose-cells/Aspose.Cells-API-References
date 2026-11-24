---
title: "TextBoxOptions.TopMarginPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt den oberen Rand zurück und legt ihn in der Einheit Punkte fest."
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Ermittelt und legt den oberen Rand in der Einheit Punkte fest.

```csharp
public double TopMarginPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Textfeld zum Arbeitsblatt hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Setze den oberen Rand in Punkten
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


