---
title: "ShapeTextAlignment.AutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Eigenschaft. Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird.

```csharp
public bool AutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Textausrichtung abrufen
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Demonstriere AutoSize = false (Standard)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // Demonstriere AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


