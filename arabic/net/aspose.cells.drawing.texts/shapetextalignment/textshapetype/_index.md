---
title: "ShapeTextAlignment.TextShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تحصل وتعيّن نوع تحويل النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

يحصل على ويضبط نوع تحويل النص.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // احصل على محاذاة النص داخل الشكل
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // تعيين الخاصية TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // احفظ المصنف
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


