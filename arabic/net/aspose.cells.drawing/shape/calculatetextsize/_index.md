---
title: "Shape.CalculateTextSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. إعادة حساب مساحة النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

إعادة حساب منطقة النص

```csharp
public int[] CalculateTextSize()
```

### قيمة الإرجاع

حجم النص في مصفوفة (العرض والارتفاع).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف نصًا تجريبيًا إلى الخلية A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // إنشاء شكل مستطيل مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // تعيين النص إلى الشكل
            shape.Text = "This is a test string to calculate text size";

            // احسب حجم النص
            int[] size = shape.CalculateTextSize();

            // أخرج النتائج
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


