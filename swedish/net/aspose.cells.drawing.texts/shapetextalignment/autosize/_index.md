---
title: "ShapeTextAlignment.AutoSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Anger om storleken på formen justeras automatiskt enligt dess innehåll"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Anger om storleken på formen justeras automatiskt enligt dess innehåll.

```csharp
public bool AutoSize { get; set; }
```

### Exempel

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

            // Lägg till en textruta
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Hämta textjustering
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Demonstrera AutoSize = false (standard)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // Demonstrera AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Spara arbetsboken
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


