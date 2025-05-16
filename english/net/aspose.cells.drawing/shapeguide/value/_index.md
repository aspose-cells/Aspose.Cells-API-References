---
title: ShapeGuide.Value
second_title: Aspose.Cells for .NET API Reference
description: ShapeGuide property. Gets or sets value of this guide
type: docs
url: /net/aspose.cells.drawing/shapeguide/value/
---
## ShapeGuide.Value property

Gets or sets value of this guide

```csharp
public double Value { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapeGuidePropertyValueDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuidePropertyValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rounded rectangle shape with default adjustments
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 200, 100, 200);

            // Access the shape's geometry adjustment guides
            if (shape.Geometry.ShapeAdjustValues.Count > 0)
            {
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[0];

                // Display current guide value (controls corner roundness percentage)
                Console.WriteLine("Initial adjustment value: " + guide.Value);

                // Modify the adjustment value to create sharper corners
                guide.Value = 0.1;  // 10% roundness
                Console.WriteLine("Updated adjustment value: " + guide.Value);

                // Add another shape to compare with original settings
                var comparisonShape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 120, 100, 200, 100, 200);
            }

            // Save the modified workbook
            workbook.Save("ShapeGuideValueDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


