---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Anger om formen ska storleksändras för att passa texten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Anger om formen ska storleksändras för att passa texten

```csharp
public bool ResizeToFitText { get; set; }
```

### Exempel

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

            // Skapa en textruta med korrekta parametrar
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // Kom åt TextBoxOptions korrekt
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Spara arbetsboken
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


