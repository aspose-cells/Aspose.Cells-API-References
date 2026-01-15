---
title: Enum ShapeTextVerticalAlignmentType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.ShapeTextVerticalAlignmentType enum. It corresponds to Format Shape  Text Options  Text Box  Vertical Alignment in Excel
type: docs
url: /net/aspose.cells.drawing.texts/shapetextverticalalignmenttype/
---
## ShapeTextVerticalAlignmentType enumeration

It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

```csharp
public enum ShapeTextVerticalAlignmentType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Top | `0` |  |
| Middle | `1` |  |
| Bottom | `2` |  |
| TopCentered | `3` |  |
| MiddleCentered | `4` |  |
| BottomCentered | `5` |  |
| Left | `6` |  |
| Center | `7` |  |
| Right | `8` |  |
| LeftMiddle | `9` |  |
| CenterMiddle | `10` |  |
| RightMiddle | `11` |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a text box to the worksheet
                var textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 300);
                textBox.Text = "Sample text for vertical alignment demonstration";

                // Set vertical text alignment to Middle
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;

                // Display the current vertical alignment
                Console.WriteLine("Current vertical alignment: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Change to Top alignment
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
                Console.WriteLine("Changed to: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Save the workbook
                workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapeTextVerticalAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


