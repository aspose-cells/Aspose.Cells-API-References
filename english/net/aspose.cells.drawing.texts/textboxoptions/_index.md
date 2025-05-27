---
title: Class TextBoxOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.TextBoxOptions class. Represents the text options of the shape
type: docs
url: /net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Represents the text options of the shape

```csharp
public class TextBoxOptions
```

## Properties

| Name | Description |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Whether allow text to overflow shape. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Returns the bottom margin in unit of Points |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Gets and sets the left margin in unit of Points. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Indicates whether to resize the shape to fit the text |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Gets and sets the right margin in unit of Points. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Gets and sets the top margin in unit of Points. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextsClassTextBoxOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.TextBoxes.Add(0, 0, 350, 350);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[index];
            textBox.Text = "Sample TextBox with Options";
            
            // Set TextBox options
            textBox.TextOptions.IsItalic = true;
            textBox.TextOptions.IsBold = true;
            textBox.TextOptions.Size = 14;
            
            // Correct way to set fill format
            textBox.FillFormat.SetOneColorGradient(System.Drawing.Color.LightBlue, 1, GradientStyleType.Horizontal, 1);
            
            textBox.LineFormat.Weight = 2;
            
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


