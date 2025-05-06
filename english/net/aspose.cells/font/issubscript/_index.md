---
title: Font.IsSubscript
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is subscript
type: docs
url: /net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Gets or sets a value indicating whether the font is subscript.

```csharp
public bool IsSubscript { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(true, cells[33, 10].GetStyle().Font.IsSubscript, caseName);
private void Property_IsSubscript(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            //compare font.name
            for (int row = 1; row &lt;= 19; row++)
            {
                Style styleSrc = cells[row, 0].GetStyle();
                Style styleDest = cells[row + 28, 0].GetStyle();
                testAreEqual(styleSrc.Font.Name, styleDest.Font.Name, caseName);
                row++;
            }
            //compare font.size
            for (int row = 1; row &lt;= 21; row++)
            {
                Style styleSrc = cells[row, 2].GetStyle();
                Style styleDest = cells[row + 28, 2].GetStyle();
                testAreEqual(styleSrc.Font.Size, styleDest.Font.Size, caseName);
                row++;
            }
            //compare font.color
            for (int row = 1; row &lt;= 19; row++)
            {
                Style styleSrc = cells[row, 4].GetStyle();
                Style styleDest = cells[row + 28, 4].GetStyle();
                testequals(styleSrc.Font.Color, styleDest.Font.Color, caseName);
            }
            //compare font.IsItalic and font.IsBold
            testAreEqual(true, cells[29, 6].GetStyle().Font.IsItalic, caseName);
            testAreEqual(true, cells[31, 6].GetStyle().Font.IsBold, caseName);
            testAreEqual(true, cells[33, 6].GetStyle().Font.IsBold, caseName);
            testAreEqual(true, cells[33, 6].GetStyle().Font.IsItalic, caseName);
            //compare underline
            for (int row = 1; row &lt;= 7; row++)
            {
                Style styleSrc = cells[row, 8].GetStyle();
                Style styleDest = cells[row + 28, 8].GetStyle();
                testAreEqual(styleSrc.Font.Underline, styleDest.Font.Underline, caseName);
                row++;
            }
            //
            testAreEqual(true, cells[29, 10].GetStyle().Font.IsStrikeout, caseName);
            testAreEqual(true, cells[31, 10].GetStyle().Font.IsSuperscript, caseName);
            testAreEqual(true, cells[33, 10].GetStyle().Font.IsSubscript, caseName);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


