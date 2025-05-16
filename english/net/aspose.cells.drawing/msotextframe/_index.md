---
title: Class MsoTextFrame
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoTextFrame class. Represents the text frame in a Shape object
type: docs
url: /net/aspose.cells.drawing/msotextframe/
---
## MsoTextFrame class

Represents the text frame in a Shape object.

```csharp
public class MsoTextFrame
```

## Properties

| Name | Description |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing/msotextframe/autosize/) { get; set; } | Indicates if size of shape is adjusted automatically according to its content. |
| [BottomMarginPt](../../aspose.cells.drawing/msotextframe/bottommarginpt/) { get; set; } | Returns the bottom margin in unit of Points |
| [IsAutoMargin](../../aspose.cells.drawing/msotextframe/isautomargin/) { get; set; } | Indicates whether the margin is auto calculated. |
| [LeftMarginPt](../../aspose.cells.drawing/msotextframe/leftmarginpt/) { get; set; } | Returns the left margin in unit of Points |
| [RightMarginPt](../../aspose.cells.drawing/msotextframe/rightmarginpt/) { get; set; } | Returns the right margin in unit of Points |
| [RotateTextWithShape](../../aspose.cells.drawing/msotextframe/rotatetextwithshape/) { get; set; } | Indicates whether rotating text with shape. |
| [TopMarginPt](../../aspose.cells.drawing/msotextframe/topmarginpt/) { get; set; } | Returns the top margin in unit of Points |

### Examples

```csharp
namespace AsposeCellsExamples.DrawingClassMsoTextFrameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMsoTextFrameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to access MsoTextFrame - fixed by adding all required parameters including height
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 2, 200, 100, 200, 100);
            
            // Configure text properties through TextBody since Shape doesn't have TextFrame
            shape.TextBody.Text = "This is a sample text demonstrating MsoTextFrame properties.\nText will auto-size and rotate with shape.";

            // Save the workbook
            workbook.Save("MsoTextFrameDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


