---
title: "TextOptions.Fill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Stellt das Füllformat des Textes dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Stellt das Füllformat des Textes dar.

```csharp
public FillFormat Fill { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Setze Schriftarteigenschaften
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Demonstriere die Fill-Eigenschaft
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


