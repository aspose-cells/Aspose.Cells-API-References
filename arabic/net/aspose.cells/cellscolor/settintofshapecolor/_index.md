---
title: "CellsColor.SetTintOfShapeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsColor. تعيين صبغة لون الشكل"
type: docs
url: /ar/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

ضبط درجة لون الشكل

```csharp
public void SetTintOfShapeColor(double tint)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ظل | Double |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // احصل على لون تعبئة الشكل
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // تعيين اللون ليُعامل كلون الشكل
                shapeColor.IsShapeColor = true;
                
                // تعيين صبغة لون الشكل (النطاق الصالح هو -1.0 إلى 1.0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // عرض التأثير عن طريق تغيير لون تعبئة الشكل
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


