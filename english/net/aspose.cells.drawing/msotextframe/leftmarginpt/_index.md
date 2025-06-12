---
title: MsoTextFrame.LeftMarginPt
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Returns the left margin in unit of Points
type: docs
url: /net/aspose.cells.drawing/msotextframe/leftmarginpt/
---
## MsoTextFrame.LeftMarginPt property

Returns the left margin in unit of Points

```csharp
public double LeftMarginPt { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating LeftMarginPt property";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current left margin
            Console.WriteLine("Current LeftMarginPt value: " + textAlignment.LeftMarginPt);

            // Set new left margin (in points)
            textAlignment.LeftMarginPt = 20.0;

            // Add more text to demonstrate the effect
            shape.Text += "\nThis text should be indented more from the left";

            // Create another shape with default margin for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text with default left margin";

            // Save the workbook
            workbook.Save("PropertyLeftMarginPtDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


