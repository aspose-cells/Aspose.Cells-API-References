---
title: Enum TextCapsType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.TextCapsType enum. This type specifies the cap types of the text
type: docs
url: /net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

This type specifies the cap types of the text.

```csharp
public enum TextCapsType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None caps |
| All | `1` | Apply all caps on the text. |
| Small | `2` | Apply small caps to the text. |

### Remarks

Only can be applied to chart and shape.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Additional code to demonstrate how the instance might be used
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set a cell's value
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Get the cell's style
            Style style = cell.GetStyle();

            // Set the font caps type to All Caps
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Apply the style to the cell
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


