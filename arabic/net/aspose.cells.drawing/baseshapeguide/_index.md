---
title: "الفئة BaseShapeGuide"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.BaseShapeGuide. تمثل دليل الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

يمثل دليل الشكل.

```csharp
public class BaseShapeGuide
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء شكل مستطيل بالمعلمات الصحيحة
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // نظرًا لأن BaseShapeGuide لا يحتوي على مُنشئ عام،
                // سنوضح استخدامه من خلال شكل قد يحتوي على guides
                // ملاحظة: هذا توضيح مبسط حيث قد يختلف الوصول الفعلي إلى الدليل
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // احفظ المصنف
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


