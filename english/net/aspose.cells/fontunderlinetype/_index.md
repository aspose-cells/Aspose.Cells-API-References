---
title: Enum FontUnderlineType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontUnderlineType enum. Enumerates the font underline types
type: docs
url: /net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Enumerates the font underline types.

```csharp
public enum FontUnderlineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Represents no underline. |
| Single | `1` | Represents single underline. |
| Double | `2` | Represents double underline. |
| Accounting | `3` | Represents single accounting underline. |
| DoubleAccounting | `4` | Represents double accounting underline. |
| Dash | `5` | Represents Dashed Underline |
| DashDotDotHeavy | `6` | Represents Thick Dash-Dot-Dot Underline |
| DashDotHeavy | `7` | Represents Thick Dash-Dot Underline |
| DashedHeavy | `8` | Represents Thick Dashed Underline |
| DashLong | `9` | Represents Long Dashed Underline |
| DashLongHeavy | `10` | Represents Thick Long Dashed Underline |
| DotDash | `11` | Represents Dash-Dot Underline |
| DotDotDash | `12` | Represents Dash-Dot-Dot Underline |
| Dotted | `13` | Represents Dotted Underline |
| DottedHeavy | `14` | Represents Thick Dotted Underline |
| Heavy | `15` | Represents Thick Underline |
| Wave | `16` | Represents Wave Underline |
| WavyDouble | `17` | Represents Double Wave Underline |
| WavyHeavy | `18` | Represents Heavy Wave Underline |
| Words | `19` | Represents Underline Non-Space Characters. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Obtain the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accessing the "A1" cell from the worksheet
            Cell cell = worksheet.Cells["A1"];
            
            // Adding some value to the "A1" cell
            cell.PutValue("Hello Aspose!");

            // Get the style of the cell
            Style style = cell.GetStyle();
            
            // Set the font underline type to single underline
            style.Font.Underline = FontUnderlineType.Single;
            
            // Apply the style to the cell
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


