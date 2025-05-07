---
title: Style.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a styles foreground color
type: docs
url: /net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Gets or sets a style's foreground color.

```csharp
public Color ForegroundColor { get; set; }
```

### Remarks

It means no color setting if Color.Empty is returned.

### Examples

```csharp
// Called: testequals(Color.Red, style.ForegroundColor, caseName);
private void Property_ForegroundColor(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row <= 5; row++)
            {
                for (int col = 2; col <= 4; col++)
                {
                    checkStyle(cells[row, col].GetStyle());
                }
            }
            Style style = cells.Rows[7].GetStyle();
            testequals(Color.Blue, style.ForegroundColor, caseName);
            testAreEqual(BackgroundType.Solid, style.Pattern, caseName);

            style = cells.Columns[6].GetStyle();
            testequals(Color.Red, style.ForegroundColor, caseName);
            testAreEqual(BackgroundType.Solid, style.Pattern, caseName);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


