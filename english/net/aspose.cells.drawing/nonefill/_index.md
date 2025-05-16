---
title: Class NoneFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.NoneFill class. Represents no fill
type: docs
url: /net/aspose.cells.drawing/nonefill/
---
## NoneFill class

Represents no fill.

```csharp
public class NoneFill : Fill
```

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |

### Examples

```csharp
namespace AsposeCellsExamples.DrawingClassNoneFillDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassNoneFillDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 2, 0, 100, 150);

            // Set fill type to None to remove shape fill
            shape.Fill.Type = FillType.None;

            // Save the workbook with transparent shape
            workbook.Save("NoneFillDemo.xlsx");
        }
    }
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


