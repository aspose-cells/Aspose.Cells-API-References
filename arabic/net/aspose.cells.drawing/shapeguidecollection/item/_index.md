---
title: "ShapeGuideCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeGuideCollection. تحصل على دليل شكل حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

يحصل على إرشاد الشكل حسب الفهرس

```csharp
public ShapeGuide this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا يستخدم أدلة التعديل
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // الوصول إلى مجموعة أدلة تعديل الشكل عبر Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // أضف أدلة جديدة إلى المجموعة
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // اعرض مثالًا على قراءة قيم الأدلة (خاصية Name غير متوفرة في التعريف المقدم)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // احفظ المصنف المعدل
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


