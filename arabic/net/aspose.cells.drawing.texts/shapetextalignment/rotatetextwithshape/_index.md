---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تشير إلى ما إذا كان يتم تدوير النص مع الشكل"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

يشير إلى ما إذا كان يتم تدوير النص مع الشكل.

```csharp
public bool RotateTextWithShape { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل صندوق نص مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // الوصول إلى خصائص محاذاة النص
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // تعيين خاصية RotateTextWithShape
            textAlignment.RotateTextWithShape = true;

            // دوران الشكل لتوضيح التأثير
            shape.RotationAngle = 45;

            // احفظ المصنف
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


