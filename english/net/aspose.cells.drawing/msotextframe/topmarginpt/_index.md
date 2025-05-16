---
title: MsoTextFrame.TopMarginPt
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Returns the top margin in unit of Points
type: docs
url: /net/aspose.cells.drawing/msotextframe/topmarginpt/
---
## MsoTextFrame.TopMarginPt property

Returns the top margin in unit of Points

```csharp
public double TopMarginPt { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoTextFramePropertyTopMarginPtDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating TopMarginPt property\nSecond line of text";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current top margin
            Console.WriteLine("Current TopMarginPt value: " + textAlignment.TopMarginPt);

            // Set new top margin (in points)
            textAlignment.TopMarginPt = 15.0;

            // Demonstrate the effect by showing the text position changes
            shape.Text += "\nThis text should appear lower due to increased top margin";

            // Save the workbook
            workbook.Save("PropertyTopMarginPtDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


