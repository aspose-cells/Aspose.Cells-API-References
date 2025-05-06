---
title: TxtLoadOptions.ExtendToNextSheet
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false
type: docs
url: /net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Remarks

If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

### Examples

```csharp
// Called: ExtendToNextSheet = true,
[Test]
        public void Property_ExtendToNextSheet()
        {
            string content = BuildExceedingCsv();
            Workbook wb = new Workbook(FileFormatType.Excel97To2003);
            Cells cells = wb.Worksheets[0].Cells;
            ImportAsCsv(cells, 0, 0, content, new TxtLoadOptions()
            {
                ExtendToNextSheet = true,
            });
            Assert.AreEqual(3, wb.Worksheets.Count, &quot;Imported sheet count&quot;);
            Assert.AreEqual(31, cells.Count, &quot;Extended sheet&apos;s cell count&quot;);
            for (int i = 0; i &lt; 256; i++)
            {
                if (i &lt; 10)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (i &lt;&lt; 1)), cells[0, i].StringValue, &quot;Col-&quot; + i);
                }
                else if (i &lt; 250)
                {
                    if (cells.CheckCell(0, i) != null)
                    {
                        Assert.Fail(&quot;Cell at column &quot; + i + &quot; should not be instantiated&quot;);
                    }
                }
                else
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + ((i - 250) &lt;&lt; 1)), cells[0, i].StringValue, &quot;Col-&quot; + i);
                }
            }
            for (int i = 1; i &lt; 65536; i++)
            {
                if (i &lt; 10)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (i &lt;&lt; 1)), cells[i, 0].StringValue, &quot;Row-&quot; + i);
                }
                else if (i &lt; 65530)
                {
                    if (cells.CheckCell(i, 0) != null)
                    {
                        Assert.Fail(&quot;Cell at row &quot; + i + &quot; should not be instantiated&quot;);
                    }
                }
                else
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + ((i - 65530) &lt;&lt; 1)), cells[i, 0].StringValue, &quot;Row-&quot; + i);
                }
            }
            cells = wb.Worksheets[1].Cells;
            Assert.AreEqual(4, cells.Count, &quot;First extended sheet&apos;s cell count&quot;);
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + ((i + 6) &lt;&lt; 1)), cells[0, i].StringValue, &quot;ExtendedCol-&quot; + i);
            }
            cells = wb.Worksheets[2].Cells;
            Assert.AreEqual(4, cells.Count, &quot;Second extended sheet&apos;s cell count&quot;);
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.AreEqual(&quot;&quot; + (char)(&apos;b&apos; + ((i + 6) &lt;&lt; 1)), cells[i, 0].StringValue, &quot;ExtendedRow-&quot; + i);
            }
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


