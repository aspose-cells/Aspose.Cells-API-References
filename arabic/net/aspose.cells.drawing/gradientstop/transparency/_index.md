---
title: "GradientStop.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientStop. تُعيد أو تُعيّن درجة الشفافية للمنطقة كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل بملء تدرج لوني
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // إنشاء لون لإيقاف التدرج
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // إضافة نقطة تدرج مع الشفافية الأولية
            gradientFill.GradientStops.Add(0, color, 30);

            // الوصول إلى إيقاف التدرج
            GradientStop stop = gradientFill.GradientStops[0];

            // عرض وتعديل الشفافية
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // إضافة نقطة أخرى للمقارنة البصرية
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // احفظ المصنف
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


