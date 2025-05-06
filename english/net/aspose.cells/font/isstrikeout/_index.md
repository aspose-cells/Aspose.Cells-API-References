---
title: Font.IsStrikeout
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is single strikeout
type: docs
url: /net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Gets or sets a value indicating whether the font is single strikeout.

```csharp
public bool IsStrikeout { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(cellsSrc[1, 10].GetStyle().Font.IsStrikeout, cellsDest[1, 10].GetStyle().Font.IsStrikeout, caseName);
private void Property_IsStrikeout(Workbook workbook)
        {
            Cells cellsSrc = workbook.Worksheets[0].Cells;
            Cells cellsDest = workbook.Worksheets[&quot;sheetDest&quot;].Cells;
            //compare font.name
            for (int row = 1; row &lt;= 19; row++)
            {
                Style styleSrc = cellsSrc[row, 0].GetStyle();
                Style styleDest = cellsDest[row, 0].GetStyle();
                testAreEqual(styleSrc.Font.Name, styleDest.Font.Name, caseName);
                row++;
            }
            //compare font.size
            for (int row = 1; row &lt;= 21; row++)
            {
                Style styleSrc = cellsSrc[row, 2].GetStyle();
                Style styleDest = cellsDest[row, 2].GetStyle();
                testAreEqual(styleSrc.Font.Size, styleDest.Font.Size, caseName);
                row++;
            }
            //compare font.color
            for (int row = 1; row &lt;= 19; row++)
            {
                Style styleSrc = cellsSrc[row, 4].GetStyle();
                Style styleDest = cellsDest[row, 4].GetStyle();
                testequals(styleSrc.Font.Color, styleDest.Font.Color, caseName);
                row++;
            }
            //compare font.isBold
            testAreEqual(cellsSrc[1, 6].GetStyle().Font.IsItalic, cellsDest[1, 6].GetStyle().Font.IsItalic, caseName);
            testAreEqual(cellsSrc[3, 6].GetStyle().Font.IsBold, cellsDest[3, 6].GetStyle().Font.IsBold, caseName);
            testAreEqual(cellsSrc[5, 6].GetStyle().Font.IsBold, cellsDest[5, 6].GetStyle().Font.IsBold, caseName);
            testAreEqual(cellsSrc[5, 6].GetStyle().Font.IsItalic, cellsDest[5, 6].GetStyle().Font.IsItalic, caseName);
            //compare Font.Underline
            for (int row = 1; row &lt;= 7; row++)
            {
                Style styleSrc = cellsSrc[row, 8].GetStyle();
                Style styleDest = cellsDest[row, 8].GetStyle();
                testAreEqual(styleSrc.Font.Underline, styleDest.Font.Underline, caseName);
                row++;
            }
            testAreEqual(cellsSrc[1, 10].GetStyle().Font.IsStrikeout, cellsDest[1, 10].GetStyle().Font.IsStrikeout, caseName);
            testAreEqual(cellsSrc[3, 10].GetStyle().Font.IsSuperscript, cellsDest[3, 10].GetStyle().Font.IsSuperscript, caseName);
            testAreEqual(cellsSrc[5, 10].GetStyle().Font.IsSubscript, cellsDest[5, 10].GetStyle().Font.IsSubscript, caseName);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


