---
title: "MsoFillFormat.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormat. تشير إلى ما إذا كان هناك ملء"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

يشير إلى ما إذا كان هناك ملء.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل نموذجي
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // تعيين رؤية الملء للشكل1 (مرئي)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // تعيين رؤية الملء للشكل2 (غير مرئي)
            shape2.FillFormat.IsVisible = false;

            // عرض استخدام خاصية IsVisible
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // مقارنة رؤية الملء بين الأشكال
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // احفظ المصنف
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


