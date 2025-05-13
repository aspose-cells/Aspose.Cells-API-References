---
title: ThreeDFormat.TopBevelHeight
second_title: Aspose.Cells for .NET API Reference
description: ThreeDFormat property. Gets and sets the height of the top bevel or how far into the shape it is applied. In unit of Points
type: docs
url: /net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points.

```csharp
public double TopBevelHeight { get; set; }
```

### Examples

```csharp
// Called: threeDFormat.TopBevelHeight = 10;
public static void ThreeDFormat_Property_TopBevelHeight()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Access the 3D format of the shape
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Set the top bevel type and dimensions
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Set the bottom bevel type and dimensions
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Save the workbook
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
```

### See Also

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


