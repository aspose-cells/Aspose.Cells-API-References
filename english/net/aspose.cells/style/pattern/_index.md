---
title: Style.Pattern
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the cell background pattern type
type: docs
url: /net/aspose.cells/style/pattern/
---
## Style.Pattern property

Gets or sets the cell background pattern type.

```csharp
public BackgroundType Pattern { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(BackgroundType.HorizontalStripe, cells[row, col].GetStyle().Pattern, &amp;quot;cells[row, col].GetStyle().Pattern&amp;quot;);
private void Property_Pattern(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row &lt;= 5; row++)
            {
                for (int col = 2; col &lt;= 3; col++)
                {
                    CheckStyle(cells[row, col].GetStyle());
                }
            }
            for (int row = 3; row &lt;= 5; row++)
            {
                for (int col = 4; col &lt;= 5; col++)
                {
                    AssertHelper.AreEqual(BackgroundType.HorizontalStripe, cells[row, col].GetStyle().Pattern, &quot;cells[row, col].GetStyle().Pattern&quot;);
                    AssertHelper.equals(Color.Green, cells[row, col].GetStyle().ForegroundColor, &quot;cells[row, col].GetStyle().ForegroundColor&quot;);
                }
            }
            Style style = cells.Rows[7].GetStyle();
            AssertHelper.equals(Color.Blue, style.ForegroundColor, &quot;cells.Rows[7].Style.ForegroundColor&quot;);
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, &quot;cells.Rows[7].Style.Pattern&quot;);
            style = cells.Columns[7].GetStyle();
            AssertHelper.equals(Color.Red, style.ForegroundColor, &quot;cells.Columns[7].Style.ForegroundColor&quot;);
            AssertHelper.AreEqual(BackgroundType.Solid, style.Pattern, &quot;cells.Columns[7].Style.Pattern&quot;);
        }
```

### See Also

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


