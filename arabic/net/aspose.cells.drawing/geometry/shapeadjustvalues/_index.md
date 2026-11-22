---
title: "Geometry.ShapeAdjustValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Geometry. يحصل على مجموعة من قيم تعديل الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/geometry/shapeadjustvalues/
---
## Geometry.ShapeAdjustValues property

يحصل على مجموعة من قيم تعديل الشكل

```csharp
public ShapeGuideCollection ShapeAdjustValues { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GeometryPropertyShapeAdjustValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Chevron, 10, 10, 0, 0, 200, 100);
            Geometry geometry = shape.Geometry;

            Console.WriteLine("Initial ShapeAdjustValues:");
            foreach (ShapeGuide guide in geometry.ShapeAdjustValues)
            {
                Console.WriteLine($"Formula: {guide.Value}");
            }

            if (geometry.ShapeAdjustValues.Count > 0)
            {
                geometry.ShapeAdjustValues[0].Value = 0.3;
                Console.WriteLine("\nModified first adjust value to 0.3");
            }

            workbook.Save("GeometryPropertyShapeAdjustValuesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeGuideCollection](../../shapeguidecollection/)
* class [Geometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


