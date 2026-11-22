---
title: "Shape.AutoShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على ويضبط نوع الشكل التلقائي"
type: docs
url: /ar/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

يحصل ويضبط نوع الشكل التلقائي.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // تحقق وعدل AutoShapeType إذا لزم الأمر
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // غيّر نوع الشكل لتوضيح الخاصية
            shape.AutoShapeType = AutoShapeType.Oval;

            // احفظ المصنف
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


