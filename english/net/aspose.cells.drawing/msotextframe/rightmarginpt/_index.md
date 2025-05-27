---
title: MsoTextFrame.RightMarginPt
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Returns the right margin in unit of Points
type: docs
url: /net/aspose.cells.drawing/msotextframe/rightmarginpt/
---
## MsoTextFrame.RightMarginPt property

Returns the right margin in unit of Points

```csharp
public double RightMarginPt { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating RightMarginPt property";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current right margin
            Console.WriteLine("Current RightMarginPt value: " + textAlignment.RightMarginPt);

            // Set new right margin (in points)
            textAlignment.RightMarginPt = 30.0;

            // Add more text to demonstrate the effect
            shape.Text += "\nThis text should have more right margin space";

            // Create another shape with default margin for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text with default right margin";

            // Save the workbook
            workbook.Save("PropertyRightMarginPtDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


