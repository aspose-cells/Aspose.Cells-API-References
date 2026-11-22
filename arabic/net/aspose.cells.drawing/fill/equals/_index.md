---
title: "Fill.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Fill. /"
type: docs
url: /ar/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف شكلاً مستطيلًا إلى ورقة العمل
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // احصل على كائن FillFormat من الشكل
                FillFormat fillFormat1 = rectangle.Fill;

                // إنشاء شكل آخر للحصول على كائن FillFormat ثاني
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // استدعاء طريقة Equals لمقارنة كائني FillFormat
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // عرض نتيجة المقارنة
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // عرض أيضًا مقارنة مع null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // احفظ المصنف
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


