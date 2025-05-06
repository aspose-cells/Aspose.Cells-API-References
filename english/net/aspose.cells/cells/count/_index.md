---
title: Cells.Count
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the total count of instantiated Cell objects
type: docs
url: /net/aspose.cells/cells/count/
---
## Cells.Count property

Gets the total count of instantiated Cell objects.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, cells.Count, &amp;quot;Imported cells count for Single&amp;quot;);
[Test]
        public void Property_Count()
        {
            Workbook wb = LoadAsCsv(&quot;a&quot;, new TxtLoadOptions());
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(1, cells.Count, &quot;Imported cells count for Single&quot;);
            Assert.AreEqual(&quot;a&quot;, cells[0, 0].StringValue, &quot;Single&quot;);
            wb = LoadAsCsv(&quot;a,a&quot;, new TxtLoadOptions());
            cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(2, cells.Count, &quot;Imported cells count for Two&quot;);
            Assert.AreEqual(&quot;a&quot;, cells[0, 0].StringValue, &quot;Two-0&quot;);
            Assert.AreEqual(&quot;a&quot;, cells[0, 1].StringValue, &quot;Two-1&quot;);
            char[] cs = new char[65560];
            for (int i = 0; i &lt; 20; i += 2)
            {
                cs[i] = (char)(&apos;a&apos; + i);
                cs[i + 1] = &apos;\n&apos;;
            }
            for (int i = 20; i &lt; 65540; i++)
            {
                cs[i] = &apos;\n&apos;;
            }
            for (int i = 65540; i &lt; 65560; i += 2)
            {
                cs[i] = (char)(&apos;b&apos; + (i - 65540));
                cs[i + 1] = &apos;\n&apos;;
                if (i &gt; 65546)
                {
                    wb = new Workbook(FileFormatType.Excel97To2003);
                    cells = wb.Worksheets[0].Cells;
                    ImportAsCsv(cells, 0, 0, new string(cs, 0, i + 1), new TxtLoadOptions() { ExtendToNextSheet = true });
                    Assert.AreEqual(Math.Min(16, 11 + ((i - 65540) &gt;&gt; 1)), cells.Count, &quot;Imported cells count for &quot; + i);
                    for (int j = Math.Min((i - 65540) &gt;&gt; 1, 6) + 65529; j &gt;= 65530; j--)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + ((j - 65530) &lt;&lt; 1)), cells[j, 0].StringValue,
                            &quot;Row-&quot; + j + &quot; for &quot; + i);
                    }
                    if (i &gt; 65550)
                    {
                        Assert.AreEqual(2, wb.Worksheets.Count, &quot;Sheet count for &quot; + i);
                        cells = wb.Worksheets[1].Cells;
                        for (int j = ((i - 65550) &gt;&gt; 1) - 6; j &gt;= 0; j--)
                        {
                            Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + 12 + (j &lt;&lt; 1)), cells[j, 0].StringValue,
                                &quot;ExtendedRow-&quot; + j + &quot; for &quot; + i);
                        }
                    }
                    else
                    {
                        Assert.AreEqual(1, wb.Worksheets.Count, &quot;Sheet count for &quot; + i);
                    }
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


