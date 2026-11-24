---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Gibt an, ob die Form so skaliert werden soll, dass der Text passt."
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Gibt an, ob die Form an den Text angepasst werden soll.

```csharp
public bool ResizeToFitText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Textfeld mit korrekten Parametern
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // Greife korrekt auf TextBoxOptions zu
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


