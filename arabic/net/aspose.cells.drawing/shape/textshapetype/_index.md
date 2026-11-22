---
title: "Shape.TextShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط نوع شكل النص المحدد مسبقًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

يحصل ويضبط نوع الشكل النصي المسبق.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // تحقق واضبط TextShapeType إذا كان غير معروف
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // أخرج TextShapeType للشكل
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### انظر أيضًا

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


