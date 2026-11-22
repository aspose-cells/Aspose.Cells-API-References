---
title: "ShapeTextAlignment.AutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تشير إلى ما إذا تم تعديل حجم الشكل تلقائيًا وفقًا لمحتواه"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتواه.

```csharp
public bool AutoSize { get; set; }
```

### أمثلة

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

            // إضافة شكل مربع نص
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // احصل على محاذاة النص
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // إظهار AutoSize = false (الافتراضي)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // إظهار AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // احفظ المصنف
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


