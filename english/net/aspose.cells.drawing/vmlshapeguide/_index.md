---
title: Class VmlShapeGuide
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.VmlShapeGuide class. just for vml Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape
type: docs
url: /net/aspose.cells.drawing/vmlshapeguide/
---
## VmlShapeGuide class

just for vml Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape

```csharp
public class VmlShapeGuide : BaseShapeGuide
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassVmlShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 200, 50);
            
            // Add the guide directly through the collection's Add method
            shape.Geometry.ShapeAdjustValues.Add("SampleGuide", 150.5);

            workbook.Save("VmlShapeGuideDemo.xlsx");
        }
    }
}
```

### See Also

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


