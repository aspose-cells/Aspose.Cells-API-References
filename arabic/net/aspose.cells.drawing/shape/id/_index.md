---
title: "Shape.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على معرف هذا الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

يحصل على معرف هذا الشكل.

```csharp
public int Id { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // احصل على وعرض معرف الشكل
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // تعديل خصائص الشكل
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // احفظ المصنف
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


