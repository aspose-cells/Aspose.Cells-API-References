---
title: StyleFlag.FontStrike
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font strikeout setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Font strikeout setting will be applied.

```csharp
public bool FontStrike { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.StyleFlagPropertyFontStrikeDemo
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and set some text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Create a style object and set FontStrike to true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Create a style flag and enable FontStrike flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Apply the style to the cell with the style flag
            cell.SetStyle(style, styleFlag);

            // Display the current FontStrike status
            Console.WriteLine("FontStrike applied: " + style.Font.IsStrikeout);

            // Create another cell to demonstrate non-strikethrough text
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");

            // Save the workbook to see the effects
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


