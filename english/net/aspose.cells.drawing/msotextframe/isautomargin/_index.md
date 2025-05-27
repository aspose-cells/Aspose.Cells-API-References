---
title: MsoTextFrame.IsAutoMargin
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Indicates whether the margin is auto calculated
type: docs
url: /net/aspose.cells.drawing/msotextframe/isautomargin/
---
## MsoTextFrame.IsAutoMargin property

Indicates whether the margin is auto calculated.

```csharp
public bool IsAutoMargin { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Sample text demonstrating IsAutoMargin property";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current IsAutoMargin value
            Console.WriteLine("Current IsAutoMargin value: " + textAlignment.IsAutoMargin);

            // Set IsAutoMargin to false to manually control margins
            textAlignment.IsAutoMargin = false;
            
            // Set custom margins (in points)
            textAlignment.LeftMarginPt = 15.0;
            textAlignment.RightMarginPt = 15.0;
            textAlignment.TopMarginPt = 10.0;
            textAlignment.BottomMarginPt = 10.0;

            // Add more text to demonstrate the effect
            shape.Text += "\nThis text has manually controlled margins";

            // Create another shape with auto margins for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text with IsAutoMargin=true (default)";
            shape2.Text += "\nMargins are automatically calculated";

            // Save the workbook
            workbook.Save("PropertyIsAutoMarginDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


