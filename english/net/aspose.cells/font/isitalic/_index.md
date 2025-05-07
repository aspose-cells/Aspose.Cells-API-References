---
title: Font.IsItalic
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is italic
type: docs
url: /net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Gets or sets a value indicating whether the font is italic.

```csharp
public bool IsItalic { get; set; }
```

### Examples

```csharp
// Called: style.Font.IsItalic = isItalics;
public static void Property_IsItalic(Workbook workbook, int sheetIndex, int startingRow, int startingColumn, int rowCount, int columnCount, string name, int size, bool isBold, bool isItalics, FontUnderlineType underline, Color color, bool isWrap)
        {
            startingRow--;
            startingColumn--;
            Style style = workbook.CreateStyle();
            style.Font.Name = name;
            style.Font.Size = size;
            style.Font.IsBold = isBold;
            style.Font.IsItalic = isItalics;
            style.Font.Underline = underline;
            style.Font.Color = color;
            style.IsTextWrapped = isWrap;
            workbook.Worksheets[sheetIndex].Cells[startingRow, startingColumn].SetStyle(style);
            Style style2 = workbook.Worksheets[sheetIndex].Cells[startingRow, startingColumn].GetStyle();
            workbook.Worksheets[sheetIndex].Cells.CreateRange(startingRow, startingColumn, rowCount, columnCount).SetStyle(style2);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


