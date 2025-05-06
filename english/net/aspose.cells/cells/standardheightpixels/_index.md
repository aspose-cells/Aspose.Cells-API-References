---
title: Cells.StandardHeightPixels
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default row height in this worksheet in unit of pixels
type: docs
url: /net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Gets or sets the default row height in this worksheet, in unit of pixels.

```csharp
public int StandardHeightPixels { get; set; }
```

### Examples

```csharp
// Called: int sh = cells.StandardHeightPixels;
[Test]
        public void Property_StandardHeightPixels()
        {
            Workbook wb = LoadAsCsv(&quot;1,2,,,5,6\n\n\n1,2,,,5,6&quot;, new TxtLoadOptions());
            Assert.AreEqual(1, wb.Worksheets.Count, &quot;Loaded sheet count&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 4; i++)
            {
                for (int j = 0; j &lt; 8; j++)
                {
                    if ((i == 0 || i == 3) &amp;&amp; (j == 0 || j == 1 || j == 4 || j == 5))
                    {
                        Assert.AreEqual(j + 1, cells[i, j].IntValue);
                    }
                    else if (cells.CheckCell(i, j) != null)
                    {
                        Assert.Fail(&quot;Cell at column &quot; + j + &quot; should not be instantiated&quot;);
                    }
                }
            }
            int sh = cells.StandardHeightPixels;
            foreach(Row r in cells.Rows)
            {
                Assert.AreEqual(sh, cells.GetRowHeightPixel(r.Index));
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


