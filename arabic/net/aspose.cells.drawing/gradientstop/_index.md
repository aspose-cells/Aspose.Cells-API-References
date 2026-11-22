---
title: "الفئة GradientStop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.GradientStop. تمثل نقطة التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

يمثل نقطة توقف التدرج.

```csharp
public class GradientStop
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | يحصل على لون نقطة التدرج هذه. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | موضع الإيقاف. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة شكل بملء تدرج لوني
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // إنشاء لون لإيقاف التدرج
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // إضافة إيقاف التدرج
                gradientFill.GradientStops.Add(0, color, 30);

                // الوصول إلى إيقاف التدرج
                GradientStop stop = gradientFill.GradientStops[0];

                // عرض الوظيفة الأساسية
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // تعديل الخصائص
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // احفظ المصنف
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


