---
title: "TextOptions.Fill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Metnin dolgu biçimini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Metnin doldurma biçimini temsil eder.

```csharp
public FillFormat Fill { get; }
```

### Örnekler

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
            
            // Yazı tipi özelliklerini ayarlayın
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Fill özelliğini göster
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


