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
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
            }
            for (int i = 1; i < 32768; i++)
            {
                cells[i, 0].PutValue(i % 1000 == 0 ? i - 1 : i);
            }
            Console.WriteLine("Test performance of FormatConditionType.DuplicateValues, time cost should be less than 3 seconds");
            //before optimization, rowsdata<>timebase: 16384<>5000; 32768<>17000; 65536<>74000;
            //after optimization:
            //  for all double values, 16384<>1000; 32768<>4000;
            //  for all int values, 16384<>160; 32768<>400;
            TimePerformance monitor = new TimePerformance(500);
            monitor.StartPerfTest();
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
            for (int i = 0; i < 10; i++)
            {
                Assert.AreEqual(16, cells[0, i].GetDisplayStyle().Font.Size, ((char)('A' + i)) + "1");
            }
            for (int i = 1; i < 32767; i++)
            {
                Assert.AreEqual(i % 1000 == 0 || (i + 1) % 1000 == 0 ? 16 : 10,
                    cells[i, 0].GetDisplayStyle().Font.Size, ((char)('A' + i)) + "1");
            }
            //Console.WriteLine("PerfBase of building cached result: " + monitor.GenPerfBase());
            monitor.FinishPerfTest("PerfBase of building cached result");
        }
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


