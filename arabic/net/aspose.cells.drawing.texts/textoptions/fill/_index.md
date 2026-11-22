---
title: "TextOptions.Fill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تمثل تنسيق التعبئة للنص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

يمثل تنسيق التعبئة للنص.

```csharp
public FillFormat Fill { get; }
```

### أمثلة

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
            
            // عيّن خصائص الخط
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // عرض خاصية Fill
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // احفظ المصنف
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


