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
namespace AsposeCellsExamples.TextsClassShapeTextVerticalAlignmentTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a text box shape
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 200, 200);
            shape.Text = "Vertical Alignment Demo";

            // Set different vertical alignment types
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.Vertical;
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.Horizontal;
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.VerticalLeftToRight;
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.Vertical90;
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.Vertical270;
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.Stacked;

            // Final alignment setting
            shape.TextBody.TextAlignment.TextVerticalType = TextVerticalType.StackedRightToLeft;

            // Save the result
            workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


