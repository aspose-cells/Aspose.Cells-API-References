---
title: "Shape.GetActualBox"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. الحصول على الموقع والحجم الفعليين للشكل بعد تطبيق الدوران أو الانعكاس وما إلى ذلك"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

احصل على الموضع الفعلي وحجم الشكل (بعد تطبيق الدوران، الانعكاس، إلخ).

```csharp
public float[] GetActualBox()
```

### قيمة الإرجاع

يعيد الموضع والحجم بالترتيب x, y, w, h

### ملاحظات

ملاحظة: الواجهة غير مكتملة الوظيفة، خاصةً أن معلومات الموقع غير صحيحة. يُنصح بعدم استخدام هذه الواجهة حتى يكتمل الوظيفة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // احصل على أبعاد الصندوق الفعلية للشكل
            float[] box = rectangle.GetActualBox();

            // إخراج أبعاد الصندوق
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // احفظ المصنف
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


