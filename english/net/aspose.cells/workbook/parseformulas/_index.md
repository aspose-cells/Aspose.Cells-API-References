---
title: Workbook.ParseFormulas
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Parses all formulas which have not been parsed when they were loaded from template file or set to a cell
type: docs
url: /net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Whether ignore error for invalid formula. For one invalid formula, if ignore error then this formula will be ignored and the process will continue to parse other formulas, otherwise exception will be thrown. |

### Examples

```csharp
// Called: wb.ParseFormulas(false);
[Test]
#endif
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            long t0 = DateTime.Now.ToFileTimeUtc();
            for (int i = 1; i &lt; 5000; i++)
            {
                cells[i, 0].Formula = @&quot;=&apos;https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1&apos;!B&quot; + i;
            }
            string rcf0 = cells[1, 0].R1C1Formula;
            t0 = DateTime.Now.ToFileTimeUtc() - t0;

            wb = new Workbook();
            cells = wb.Worksheets[0].Cells;
            wb.StartAccessCache(AccessCacheOptions.SetFormula);
            long t1 = DateTime.Now.ToFileTimeUtc();
            for (int i = 1; i &lt; 5000; i++)
            {
                cells[i, 0].Formula = @&quot;=&apos;https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1&apos;!B&quot; + i;
            }
            wb.CloseAccessCache(AccessCacheOptions.SetFormula);
            string rcf1 = cells[1, 0].R1C1Formula;
            t1 = DateTime.Now.ToFileTimeUtc() - t1;
            Assert.AreEqual(rcf0, rcf1, &quot;RCFormula&quot;);
            if (t1 &gt;= t0 || t1 &gt; ((t0 - t1) &lt;&lt; 1)) // 2/3;
            {
                Assert.Fail(&quot;Time cost of cached-parse[&quot; + (t1 / 10000) + &quot;ms] should be less than normal[&quot; + (t0 / 10000) + &quot;ms]&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Time cost of cached-parse[&quot; + (t1 / 10000) + &quot;ms], normal[&quot; + (t0 / 10000) + &quot;ms]&quot;);
            }

            wb = new Workbook();
            cells = wb.Worksheets[0].Cells;
            t1 = DateTime.Now.ToFileTimeUtc();
            for (int i = 1; i &lt; 5000; i++)
            {
                cells[i, 0].SetFormula(@&quot;=&apos;https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1&apos;!B&quot; + i,
                    new FormulaParseOptions() {Parse = false}, null);
            }
            Console.WriteLine(&quot;Time cost of setting formulas without parse: &quot; + ((DateTime.Now.ToFileTimeUtc() - t1) / 10000));
            wb.ParseFormulas(false);
            Console.WriteLine(&quot;Time cost of setting and parsing formulas: &quot; + ((DateTime.Now.ToFileTimeUtc() - t1) / 10000));
            rcf1 = cells[1, 0].R1C1Formula;
            t1 = DateTime.Now.ToFileTimeUtc() - t1;
            Assert.AreEqual(rcf0, rcf1, &quot;RCFormula&quot;);
            if (t1 &gt;= t0 || t0 &gt; (t0 - t1) &lt;&lt; 2) // 3/4; t1 &gt; ((t0 - t1) &lt;&lt; 1) // 2/3
            {
                Assert.Fail(&quot;Time cost of batch-parse[&quot; + (t1 / 10000) + &quot;ms] should be much less than normal[&quot; + (t0 / 10000) + &quot;ms]&quot;);
            }
            else
            {
                Console.WriteLine(&quot;Time cost of batch-parse[&quot; + (t1 / 10000) + &quot;ms], normal[&quot; + (t0 / 10000) + &quot;ms]&quot;);
            }
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


