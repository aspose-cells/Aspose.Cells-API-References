---
title: Border.Color
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets or sets the Color of the border
type: docs
url: /net/aspose.cells/border/color/
---
## Border.Color property

Gets or sets the Color of the border.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: testequals(styleSrc.Borders[BorderType.LeftBorder].Color, styleDest.Borders[BorderType.LeftBorder].Color, caseName);
private void Border_Property_Color(Workbook workbook)
        {
            Cells cellsSrc = workbook.Worksheets[0].Cells;
            Cells cellsDest = workbook.Worksheets["sheetDest"].Cells;
            for (int row = 1; row <= 25; row++)
            {
                Style styleSrc = cellsSrc[row, 1].GetStyle();
                Style styleDest = cellsDest[row, 1].GetStyle();
                //compare bordersetting
                testequals(styleSrc.Borders[BorderType.TopBorder].Color, styleDest.Borders[BorderType.TopBorder].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.TopBorder].LineStyle, styleDest.Borders[BorderType.TopBorder].LineStyle, caseName);
                testequals(styleSrc.Borders[BorderType.LeftBorder].Color, styleDest.Borders[BorderType.LeftBorder].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.LeftBorder].LineStyle, styleDest.Borders[BorderType.LeftBorder].LineStyle, caseName);
                testequals(styleSrc.Borders[BorderType.RightBorder].Color, styleDest.Borders[BorderType.RightBorder].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.RightBorder].LineStyle, styleDest.Borders[BorderType.RightBorder].LineStyle, caseName);
                testequals(styleSrc.Borders[BorderType.BottomBorder].Color, styleDest.Borders[BorderType.BottomBorder].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.BottomBorder].LineStyle, styleDest.Borders[BorderType.BottomBorder].LineStyle, caseName);
                testequals(styleSrc.Borders[BorderType.DiagonalDown].Color, styleDest.Borders[BorderType.DiagonalDown].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.DiagonalDown].LineStyle, styleDest.Borders[BorderType.DiagonalDown].LineStyle, caseName);
                testequals(styleSrc.Borders[BorderType.DiagonalUp].Color, styleDest.Borders[BorderType.DiagonalUp].Color, caseName);
                testAreEqual(styleSrc.Borders[BorderType.DiagonalUp].LineStyle, styleDest.Borders[BorderType.DiagonalUp].LineStyle, caseName);
                row++;
            }
        }
```

### See Also

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


