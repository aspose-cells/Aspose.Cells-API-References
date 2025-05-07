---
title: Font.IsNormalizeHeights
second_title: Aspose.Cells for .NET API Reference
description: Font property. Indicates whether the normalization of height that is to be applied to the text run
type: docs
url: /net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Indicates whether the normalization of height that is to be applied to the text run.

```csharp
public bool IsNormalizeHeights { get; set; }
```

### Examples

```csharp
// Called: font.IsNormalizeHeights = false;
public static void Property_IsNormalizeHeights()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // Accessing the "A1" cell from the worksheet
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Adding some value to the "A1" cell
            cell.PutValue("Hello Aspose!");

            // Accessing the font object of the cell style
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Setting the font name to "Times New Roman"
            font.Name = "Times New Roman";

            // Setting font size to 14
            font.Size = 14;

            // Setting font color as Red
            font.Color = Color.Red;

            // Setting additional font properties
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Saving the Excel file
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


