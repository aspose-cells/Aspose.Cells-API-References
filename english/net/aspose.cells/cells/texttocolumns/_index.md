---
title: Cells.TextToColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Splits content in specified column into multiple columns
type: docs
url: /net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Splits content in specified column into multiple columns..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| totalRows | Int32 | The number of rows. |
| options | TxtLoadOptions | The split options. |

### Return Value

Total column count of the split values.

### Examples

```csharp
// Called: int cc = cells.TextToColumns(9, 1, 5, opts);
[Test]
        public void Method_TxtLoadOptions_()
        { //and 46155
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 2; i++)
            {
                cells.Clear();
                cells[10, 1].PutValue(&quot;a&amp;b&amp;c&amp;1,234.56&quot;);
                cells[12, 1].PutValue(&quot;ab&amp;cd&quot;);
                TxtLoadOptions opts = new TxtLoadOptions();
                opts.Separator = &apos;&amp;&apos;;
                if (i &gt; 0)
                {
                    opts.LoadStyleStrategy = TxtLoadStyleStrategy.None;
                }
                int cc = cells.TextToColumns(9, 1, 5, opts);
                Assert.AreEqual(4, cc, &quot;Split column count&quot;);
                Assert.AreEqual(&quot;a&quot;, cells[10, 1].StringValue, &quot;B11&quot;);
                Assert.AreEqual(&quot;b&quot;, cells[10, 2].StringValue, &quot;C11&quot;);
                Assert.AreEqual(&quot;c&quot;, cells[10, 3].StringValue, &quot;D11&quot;);
                if (i &gt; 0)
                {
                    Assert.AreEqual(&quot;1234.56&quot;, cells[10, 4].StringValue, &quot;With strategy None, E11.StringValue&quot;);
                }
                else
                {
                    Assert.AreEqual(&quot;1,234.56&quot;, cells[10, 4].StringValue, &quot;Without strategy, E11.StringValue&quot;);
                }
                Assert.AreEqual(1234.56, cells[10, 4].DoubleValue, &quot;E11.DoubleValue&quot;);
                Assert.AreEqual(&quot;ab&quot;, cells[12, 1].StringValue, &quot;B13&quot;);
                Assert.AreEqual(&quot;cd&quot;, cells[12, 2].StringValue, &quot;C13&quot;);
            }
        }
```

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


