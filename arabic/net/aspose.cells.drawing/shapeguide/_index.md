---
title: "الفئة ShapeGuide"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.ShapeGuide فئة. تغلف دليل الشكل الذي يحدد وجود دليل شكل سيُستخدم للتحكم في هندسة الشكل المحدد."
type: docs
url: /ar/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

يغلف دليل الشكل الذي يحدد وجود دليل شكل سيُستخدم للتحكم في هندسة الشكل المحدد

```csharp
public class ShapeGuide : BaseShapeGuide
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | يحصل على أو يضبط قيمة هذا الدليل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // أنشئ وأضف دليل الشكل مع المعلمات المطلوبة
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


