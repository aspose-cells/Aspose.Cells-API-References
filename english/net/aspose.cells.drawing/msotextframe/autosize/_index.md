---
title: MsoTextFrame.AutoSize
second_title: Aspose.Cells for .NET API Reference
description: MsoTextFrame property. Indicates if size of shape is adjusted automatically according to its content
type: docs
url: /net/aspose.cells.drawing/msotextframe/autosize/
---
## MsoTextFrame.AutoSize property

Indicates if size of shape is adjusted automatically according to its content.

```csharp
public bool AutoSize { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoTextFramePropertyAutoSizeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class MsoTextFramePropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with text frame
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            shape.Text = "Initial text content";

            // Access the MsoTextFrame through TextBody's TextAlignment
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;

            // Display current AutoSize value
            Console.WriteLine("Current AutoSize value: " + textAlignment.AutoSize);

            // Set AutoSize to true
            textAlignment.AutoSize = true;

            // Add more text to demonstrate automatic resizing
            shape.Text += "\nAdding more text to demonstrate AutoSize functionality. " +
                         "The shape should automatically adjust its size to fit this content.";

            // Create another shape with AutoSize set to false for comparison
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 5, 200, 100, 200, 100);
            shape2.Text = "Text with AutoSize=false - content may be clipped";
            shape2.TextBody.TextAlignment.AutoSize = false;
            shape2.Text += "\nAdditional text that won't cause automatic resizing";

            // Save the workbook
            workbook.Save("PropertyAutoSizeDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoTextFrame](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


