---
title: Class GroupFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GroupFill class. Represents this fill format should inherit the fill properties of the group
type: docs
url: /net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Represents this fill format should inherit the fill properties of the group.

```csharp
public class GroupFill : Fill
```

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add two rectangle shapes to the worksheet
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 50, 100, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 50, 100, 100, 50);

            // Group the shapes into a single group shape
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Access first sub-shape in the group
            Shape groupedShape1 = groupShape.GetGroupedShapes()[0];

            // Configure group's fill properties (inherited by GroupFill)
            groupShape.Fill.SolidFill.Color = Color.CornflowerBlue;

            // Configure second sub-shape with explicit fill (non-inherited)
            groupShape.GetGroupedShapes()[1].Fill.SolidFill.Color = Color.LightGreen;

            // Save the modified workbook
            workbook.Save("GroupFillDemo.xlsx");
        }
    }
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


