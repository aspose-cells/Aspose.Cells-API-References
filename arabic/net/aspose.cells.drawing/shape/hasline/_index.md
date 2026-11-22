---
title: "Shape.HasLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط ما إذا كان حد الخط للشكل مرئيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

يحصل أو يحدد ظهور حد الخط للشكل.

```csharp
public bool HasLine { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // عرض خاصية HasLine
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // إزالة الخط
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // إعادة إضافة الخط
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


