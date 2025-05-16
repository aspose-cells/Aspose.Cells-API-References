---
title: ShapeGuideCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ShapeGuideCollection property. Gets a shape guide by index
type: docs
url: /net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Gets a shape guide by index

```csharp
public ShapeGuide this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index |  |

### Examples

```csharp
namespace AsposeCellsExamples.ShapeGuideCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape that uses adjustment guides
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 100, 100);
            shape.AutoShapeType = AutoShapeType.Rectangle;

            // Access the shape's adjustment guides collection via Geometry
            ShapeGuideCollection guides = shape.Geometry.ShapeAdjustValues;

            // Add new guides to the collection
            guides.Add("WidthGuide", 50.0);
            guides.Add("HeightGuide", 75.0);

            // Demonstrate reading guide values (Name property not available in provided definition)
            Console.WriteLine("First guide value: " + guides[0].Value);
            Console.WriteLine("\nSecond guide value: " + guides[1].Value);

            // Save the modified workbook
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


