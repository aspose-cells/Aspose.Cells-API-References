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
            for (int i = 1; i < 5000; i++)
            {
                cells[i, 0].Formula = @"='https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1'!B" + i;
            }
            string rcf0 = cells[1, 0].R1C1Formula;
            t0 = DateTime.Now.ToFileTimeUtc() - t0;

            wb = new Workbook();
            cells = wb.Worksheets[0].Cells;
            wb.StartAccessCache(AccessCacheOptions.SetFormula);
            long t1 = DateTime.Now.ToFileTimeUtc();
            for (int i = 1; i < 5000; i++)
            {
                cells[i, 0].Formula = @"='https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1'!B" + i;
            }
            wb.CloseAccessCache(AccessCacheOptions.SetFormula);
            string rcf1 = cells[1, 0].R1C1Formula;
            t1 = DateTime.Now.ToFileTimeUtc() - t1;
            Assert.AreEqual(rcf0, rcf1, "RCFormula");
            if (t1 >= t0 || t1 > ((t0 - t1) << 1)) // 2/3;
            {
                Assert.Fail("Time cost of cached-parse[" + (t1 / 10000) + "ms] should be less than normal[" + (t0 / 10000) + "ms]");
            }
            else
            {
                Console.WriteLine("Time cost of cached-parse[" + (t1 / 10000) + "ms], normal[" + (t0 / 10000) + "ms]");
            }

            wb = new Workbook();
            cells = wb.Worksheets[0].Cells;
            t1 = DateTime.Now.ToFileTimeUtc();
            for (int i = 1; i < 5000; i++)
            {
                cells[i, 0].SetFormula(@"='https:\\www.aspose.com\sub1\sub2\[testPointed.xlsx]Sheet1'!B" + i,
                    new FormulaParseOptions() {Parse = false}, null);
            }
            Console.WriteLine("Time cost of setting formulas without parse: " + ((DateTime.Now.ToFileTimeUtc() - t1) / 10000));
            wb.ParseFormulas(false);
            Console.WriteLine("Time cost of setting and parsing formulas: " + ((DateTime.Now.ToFileTimeUtc() - t1) / 10000));
            rcf1 = cells[1, 0].R1C1Formula;
            t1 = DateTime.Now.ToFileTimeUtc() - t1;
            Assert.AreEqual(rcf0, rcf1, "RCFormula");
            if (t1 >= t0 || t0 > (t0 - t1) << 2) // 3/4; t1 > ((t0 - t1) << 1) // 2/3
            {
                Assert.Fail("Time cost of batch-parse[" + (t1 / 10000) + "ms] should be much less than normal[" + (t0 / 10000) + "ms]");
            }
            else
            {
                Console.WriteLine("Time cost of batch-parse[" + (t1 / 10000) + "ms], normal[" + (t0 / 10000) + "ms]");
            }
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


