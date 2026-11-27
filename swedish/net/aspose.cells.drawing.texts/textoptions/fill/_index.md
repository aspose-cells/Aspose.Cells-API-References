---
title: "TextOptions.Fill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Representerar fyllningsformatet för texten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Representerar fyllningsformatet för texten.

```csharp
public FillFormat Fill { get; }
```

### Exempel

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
            
            // Ställ in teckensnittsegenskaper
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Demonstrera Fill-egenskap
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Spara arbetsboken
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


