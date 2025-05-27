---
title: MsoTextFrame.RotateTextWithShape
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Indicates whether rotating text with shape
type: docs
url: /net/aspose.cells.drawing/msotextframe/rotatetextwithshape/
---
## MsoTextFrame.RotateTextWithShape property

Indicates whether rotating text with shape.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating RotateTextWithShape property";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current RotateTextWithShape value
            Console.WriteLine("Current RotateTextWithShape value: " + textAlignment.RotateTextWithShape);

            // Set RotateTextWithShape to true
            textAlignment.RotateTextWithShape = true;

            // Rotate the shape to demonstrate the effect
            shape.RotationAngle = 45;

            // Add another shape with RotateTextWithShape set to false for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text without rotation (RotateTextWithShape=false)";
            shape2.TextBody.TextAlignment.RotateTextWithShape = false;
            shape2.RotationAngle = 45;

            // Save the workbook
            workbook.Save("PropertyRotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


