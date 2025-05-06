---
title: TxtLoadOptions.MaxColumnCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The maximum count of columns to be imported for one sheet
type: docs
url: /net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

The maximum count of columns to be imported for one sheet.

```csharp
public int MaxColumnCount { get; set; }
```

### Remarks

Those columns exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header columns([`HeaderColumnsCount`](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### Examples

```csharp
// Called: tailCol = opts.MaxColumnCount - opts.HeaderColumnsCount;
[Test]
        public void Property_MaxColumnCount()
        {
            char[] cs = new char[450];
            for (int i = 0; i &lt; cs.Length; i += 2)
            {
                cs[i] = i % 50 == 0 ? &apos;\n&apos; : &apos;,&apos;;
                cs[i + 1] = (char)(&apos;a&apos; + ((i &gt;&gt; 1) % 26));
            }
            string content = new string(cs, 1, cs.Length - 1);
            TxtLoadOptions opts = new TxtLoadOptions()
            {
                Encoding = Encoding.Unicode,
                ExtendToNextSheet = true,
                HeaderRowsCount = 2,
                HeaderColumnsCount = 3,
                MaxRowCount = 6,
                MaxColumnCount = 8
            };
            MemoryStream ms = new MemoryStream(Encoding.Unicode.GetBytes(content), false);
            Workbook wb = new Workbook(ms, opts);
            int tailRow = cs.Length / 50 - opts.MaxRowCount;
            int tailCol = opts.MaxRowCount - opts.HeaderRowsCount;
            int sheetCount = (tailRow + tailCol - 1) / tailCol + 1;
            tailRow = (tailRow % tailCol) + opts.HeaderRowsCount;
            tailCol = opts.MaxColumnCount - opts.HeaderColumnsCount;
            sheetCount *= (25 - opts.MaxColumnCount + tailCol - 1) / tailCol + 1;
            tailCol = ((25 - opts.MaxColumnCount) % tailCol) + opts.HeaderColumnsCount;
            Assert.AreEqual(sheetCount, wb.Worksheets.Count, &quot;Data should be expanded to 10 sheets&quot;);
            Cells cells;
            string sn;
            for (int s = 0; s &lt; (sheetCount &gt;&gt; 1); s++)
            {
                cells = wb.Worksheets[s].Cells;
                sn = &quot;Sheet&quot; + (s + 1) + &quot;!&quot;;
                for (int r = 0; r &lt; opts.MaxRowCount; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 4 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (26 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
            }
            for (int s = (sheetCount &gt;&gt; 1); s &lt; sheetCount; s++)
            {
                cells = wb.Worksheets[s].Cells;
                sn = &quot;Sheet&quot; + (s + 1) + &quot;!&quot;;
                for (int r = 0; r &lt; opts.HeaderRowsCount; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 9 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (1 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
                for (int r = opts.HeaderRowsCount; r &lt; tailRow; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c - 4) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 9 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (23 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
            }

            wb = new Workbook(FileFormatType.Excel97To2003);
            ms.Seek(0, SeekOrigin.Begin);
            wb.Worksheets[0].Cells.ImportCSV(ms, opts, 65532, 252);

            sheetCount = 16;
            cells = wb.Worksheets[0].Cells;
            sn = &quot;Sheet1!&quot;;
            for (int r = 65532; r &lt; 65536; r++)
            {
                for (int c = 252; c &lt; 256; c++)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + ((r - 65532) * 25 + c - 252) % 26),
                        cells[r, c].StringValue, sn + CellsHelper.CellIndexToName(r, c));
                }
            }
            for (int s = 1; s &lt; 6; s++)
            {
                cells = wb.Worksheets[s].Cells;
                sn = &quot;Sheet&quot; + (s + 1) + &quot;!&quot;;
                for (int r = 0; r &lt; 4; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 5 ? 8 : 4); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (22 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
            }
            cells = wb.Worksheets[5].Cells;
            sn = &quot;Sheet6!&quot;;
            for (int r = 0; r &lt; 4; r++)
            {
                for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                        sn + CellsHelper.CellIndexToName(r, c));
                }
                Assert.AreEqual(&quot;&quot; + (char)(&apos;y&apos; - r), cells[r, opts.HeaderColumnsCount].StringValue,
                    sn + CellsHelper.CellIndexToName(r, opts.HeaderColumnsCount));
            }
            for (int s = 6; s &lt; 11; s++)
            {
                cells = wb.Worksheets[s].Cells;
                sn = &quot;Sheet&quot; + (s + 1) + &quot;!&quot;;
                for (int r = 0; r &lt; opts.HeaderRowsCount; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 10 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (s * 5 + c - 30 - r) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
                for (int r = opts.HeaderRowsCount; r &lt; 6; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c - 28) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 10 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + ((s - 6) * 5 + r * 25 + c - 2) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
            }
            for (int s = 11; s &lt; 16; s++)
            {
                cells = wb.Worksheets[s].Cells;
                sn = &quot;Sheet&quot; + (s + 1) + &quot;!&quot;;
                for (int r = 0; r &lt; opts.HeaderRowsCount; r++)
                {
                    for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (r * 25 + c) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                    for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 15 ? 8 : 5); c++)
                    {
                        Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (s * 5 + c - 29 - r) % 26), cells[r, c].StringValue,
                            sn + CellsHelper.CellIndexToName(r, c));
                    }
                }
                for (int c = 0; c &lt; opts.HeaderColumnsCount; c++)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + (18 + c) % 26), cells[2, c].StringValue,
                        sn + CellsHelper.CellIndexToName(2, c));
                }
                for (int c = opts.HeaderColumnsCount; c &lt; (s &lt; 15 ? 8 : 5); c++)
                {
                    Assert.AreEqual(&quot;&quot; + (char)(&apos;a&apos; + ((s - 6) * 5 + 19 + c) % 26), cells[2, c].StringValue,
                        sn + CellsHelper.CellIndexToName(2, c));
                }
            }
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


