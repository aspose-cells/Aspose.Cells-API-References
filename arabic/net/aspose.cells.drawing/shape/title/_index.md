---
title: "Shape.Title"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحدد تسمية العنوان لكائن الشكل الحالي"
type: docs
url: /ar/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

يحدد العنوان (التسمية) لكائن الشكل الحالي.

```csharp
public string Title { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // قم بتعيين عنوان الشكل
            shape.Title = "title1";

            // تحقق من أن العنوان تم تعيينه
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


