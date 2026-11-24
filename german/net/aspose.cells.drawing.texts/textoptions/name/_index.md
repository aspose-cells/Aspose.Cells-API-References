---
title: "TextOptions.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions property. Gibt den Namen der Form zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/name/
---
## TextOptions.Name property

Liest und setzt den Namen der Form.

```csharp
public override string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            textOptions.Color = System.Drawing.Color.Blue;
            
            workbook.Save("TextOptionsPropertyNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


