---
title: "GradientFill.SetGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GradientFill. تعيين نوع تعبئة التدرج والاتجاه"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

تعيين نوع تعبئة التدرج والاتجاه.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | GradientFillType | نوع تعبئة التدرج. |
| angle | Double | الزاوية. ينطبق فقط على GradientFillType.Linear. |
| direction | GradientDirectionType | نوع الاتجاه. ينطبق فقط على GradientFillType.Radial و GradientFillType.Rectangle. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل لتطبيق ملء التدرّج
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // احصل على تدرج تعبئة الشكل
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // استدعاء SetGradient مع معلمات محددة: تعبئة خطية، 90 درجة، اتجاه FromCenter
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // احفظ المصنف لتوضيح التأثير
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


