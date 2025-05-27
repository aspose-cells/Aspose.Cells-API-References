---
title: Class AutomaticFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.AutomaticFill class. represents automatic fill
type: docs
url: /net/aspose.cells.drawing/automaticfill/
---
## AutomaticFill class

represents automatic fill.

```csharp
public class AutomaticFill : Fill
```

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class AutomaticFillDemo
    {
        public static void RunDemo()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Add a shape to the worksheet
            Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);

            // Set the fill format of the shape to AutomaticFill
            shape.Fill.FillType = FillType.Automatic;

            // Save the workbook
            workbook.Save("AutomaticFillDemo.xlsx");

            shape.Fill.FillType = FillType.Pattern;
            shape.Fill.Pattern = FillPattern.SolidDiamond;
            shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Red;
            shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Green;

            workbook.Save("PatternFillDemo2.xlsx");
            workbook.Save("PatternFillDemo2.pdf");
        }
    }
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


