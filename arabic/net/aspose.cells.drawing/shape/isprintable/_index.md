---
title: "Shape.IsPrintable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False فلن يتم طباعة هذا الشكل عند الطباعة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

يشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False، فلن يُطبع هذا الشكل عند الطباعة.

```csharp
public bool IsPrintable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // عرض خاصية IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // تبديل خاصية IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // تعيين IsPrintable إلى false صراحةً
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


