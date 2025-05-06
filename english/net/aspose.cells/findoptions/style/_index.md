---
title: FindOptions.Style
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. The format to search for
type: docs
url: /net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

The format to search for.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: options.Style = style;
[Test]
        public void Property_Style()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style style = wb.CreateStyle();
            Border b = style.Borders[BorderType.TopBorder];
            b.Color = Color.Red;
            b.LineStyle = CellBorderType.Double;
            cells[0, 0].SetStyle(style);
            cells[0, 3].SetStyle(style);
            cells[4, 1].SetStyle(style);
            b.Color = Color.Blue;
            cells[0, 1].SetStyle(style);
            cells[2, 1].SetStyle(style);
            b.Color = Color.Red;
            FindOptions options = new FindOptions();
            options.Style = style;
            Cell nextCell = null;
            int[] rcs = new[] {0, 0, 0, 3, 4, 1};
            int offset = 0;
            while (true)
            {
                nextCell = cells.Find(null, nextCell, options);
                if (nextCell == null)
                {
                    if (offset &lt; rcs.Length)
                    {
                        Assert.Fail(&quot;Cannot find cell[&quot; + rcs[offset] + &quot;,&quot; + rcs[offset+1] + &quot;]&quot;);
                    }
                    break;
                }
                if (nextCell.Row != rcs[offset] || nextCell.Column != rcs[offset + 1])
                {
                    Assert.Fail(&quot;Expected cell[&quot; + rcs[offset] + &quot;,&quot; + rcs[offset + 1]
                        + &quot;] but was [&quot; + nextCell.Row + &quot;,&quot; + nextCell.Column + &quot;]&quot;);
                }
                offset += 2;
            }
        }
```

### See Also

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


