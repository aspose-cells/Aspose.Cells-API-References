---
title: "GradientStop.CellsColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientStop. تحصل على لون هذه النقطة التدرجية"
type: docs
url: /ar/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

يحصل على لون نقطة التدرج هذه.

```csharp
public CellsColor CellsColor { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
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

                // الوصول إلى نقطة التدرج وعرض خصائص CellsColor الخاصة بها
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // احفظ المصنف
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


