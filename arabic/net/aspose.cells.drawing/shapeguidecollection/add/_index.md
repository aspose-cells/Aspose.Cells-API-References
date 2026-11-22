---
title: "ShapeGuideCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeGuideCollection. تُضيف دليل شكل. مهم: هذه الميزة متاحة حاليًا فقط لـ Excel07 وما فوق"
type: docs
url: /ar/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

يضيف إرشادًا للشكل.(مهم: هذه الميزة متاحة حاليًا فقط لإصدارات Excel07 وما فوق)

```csharp
public int Add(string name, double val)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم التعديل. هو كما \"adj(Used when there is only one adjustment value)\", \"adj1\", \"adj2\", \"adj3\" وهكذا. |
| val | Double | قيمة التعديل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ شكلًا يستخدم أدلة التعديل
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // احصل على ShapeGuideCollection من تعديلات هندسة الشكل
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // استدعِ طريقة Add مع معلمات (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


