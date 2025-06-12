---
title: Class BaseShapeGuide
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.BaseShapeGuide class. Represents the shape guide
type: docs
url: /net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Represents the shape guide.

```csharp
public class BaseShapeGuide
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape and get its geometry
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 150, 0, 0);
            Geometry geometry = shape.Geometry;

            // Create and configure shape guides using collection's Add method
            geometry.ShapeAdjustValues.Add("WidthGuide", 0.0);
            geometry.ShapeAdjustValues.Add("HeightGuide", 0.0);

            // Save with guides added (visible in generated XML)
            workbook.Save("BaseShapeGuideDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


