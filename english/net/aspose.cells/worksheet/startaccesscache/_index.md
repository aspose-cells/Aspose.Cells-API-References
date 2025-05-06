---
title: Worksheet.StartAccessCache
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Starts the session that uses caches to access the data in this worksheet
type: docs
url: /net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Starts the session that uses caches to access the data in this worksheet.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |

### Remarks

After finishing the access to the data, [`CloseAccessCache`](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.

### Examples

```csharp
// Called: sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
[Test]
        public void Method_AccessCacheOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 65536, 9));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;
            Cells cells = sheet.Cells;
            for (int i = 0; i &lt; 10; i++)
            {
                cells[0, i].PutValue(&quot;A&quot;);
            }
            for (int i = 1; i &lt; 32768; i++)
            {
                cells[i, 0].PutValue(i % 1000 == 0 ? i - 1 : i);
            }
            Console.WriteLine(&quot;Test performance of FormatConditionType.DuplicateValues, time cost should be less than 3 seconds&quot;);
            //before optimization, rowsdata&lt;&gt;timebase: 16384&lt;&gt;5000; 32768&lt;&gt;17000; 65536&lt;&gt;74000;
            //after optimization:
            //  for all double values, 16384&lt;&gt;1000; 32768&lt;&gt;4000;
            //  for all int values, 16384&lt;&gt;160; 32768&lt;&gt;400;
            TimePerformance monitor = new TimePerformance(500);
            monitor.StartPerfTest();
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
            for (int i = 0; i &lt; 10; i++)
            {
                Assert.AreEqual(16, cells[0, i].GetDisplayStyle().Font.Size, ((char)(&apos;A&apos; + i)) + &quot;1&quot;);
            }
            for (int i = 1; i &lt; 32767; i++)
            {
                Assert.AreEqual(i % 1000 == 0 || (i + 1) % 1000 == 0 ? 16 : 10,
                    cells[i, 0].GetDisplayStyle().Font.Size, ((char)(&apos;A&apos; + i)) + &quot;1&quot;);
            }
            //Console.WriteLine(&quot;PerfBase of building cached result: &quot; + monitor.GenPerfBase());
            monitor.FinishPerfTest(&quot;PerfBase of building cached result&quot;);
        }
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


