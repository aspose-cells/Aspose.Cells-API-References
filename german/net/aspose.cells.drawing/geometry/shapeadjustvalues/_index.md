---
title: "Geometry.ShapeAdjustValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Geometry-Eigenschaft. Gibt eine Sammlung von Form-Anpassungswerten zurück"
type: docs
url: /de/net/aspose.cells.drawing/geometry/shapeadjustvalues/
---
## Geometry.ShapeAdjustValues property

Ruft eine Sammlung von Formanpassungswerten ab

```csharp
public ShapeGuideCollection ShapeAdjustValues { get; }
```

### Beispiele

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

### Siehe auch

* class [ShapeGuideCollection](../../shapeguidecollection/)
* class [Geometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


