---
title: MsoTextFrame.BottomMarginPt
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Returns the bottom margin in unit of Points
type: docs
url: /net/aspose.cells.drawing/msotextframe/bottommarginpt/
---
## MsoTextFrame.BottomMarginPt property

Returns the bottom margin in unit of Points

```csharp
public double BottomMarginPt { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating BottomMarginPt property\nFirst line\nSecond line\nThird line";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current bottom margin
            Console.WriteLine("Current BottomMarginPt value: " + textAlignment.BottomMarginPt);

            // Set new bottom margin (in points)
            textAlignment.BottomMarginPt = 30.0;

            // Add more text to demonstrate the effect
            shape.Text += "\nThis text should appear higher due to increased bottom margin";

            // Create another shape with default margin for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text with default bottom margin\nFirst line\nSecond line\nThird line";

            // Save the workbook
            workbook.Save("PropertyBottomMarginPtDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


