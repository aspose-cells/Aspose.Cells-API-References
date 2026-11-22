---
title: "GradientFill.GradientStops"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientFill. تمثّل مجموعة نقاط التدرّج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

يمثل مجموعة نقاط توقف التدرج.

```csharp
public GradientStopCollection GradientStops { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyGradientStopsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            
            // إضافة شكل مستطيل
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // تعيين ملء التدرّج
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // مسح أي نقاط تدرّج موجودة
            gradientFill.GradientStops.Clear();

            // إضافة نقاط تدرّج مخصصة
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // عرض الوصول إلى نقاط التدرّج
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


