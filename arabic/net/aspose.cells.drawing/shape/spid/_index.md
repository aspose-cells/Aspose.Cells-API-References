---
title: "Shape.Spid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحدد معرف سلسلة اختياري يمكن للتطبيق استخدامه لتحديد الشكل المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

يحدد معرف سلسلة اختياري يمكن للتطبيق استخدامه لتحديد الشكل المحدد.

```csharp
public string Spid { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل إلى ورقة العمل مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // الحصول على خاصية Spid للشكل وعرضها
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // احفظ المصنف
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


