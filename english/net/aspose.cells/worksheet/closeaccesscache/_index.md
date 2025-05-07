---
title: Worksheet.CloseAccessCache
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Closes the session that uses caches to access the data in this worksheet
type: docs
url: /net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Closes the session that uses caches to access the data in this worksheet.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |

### Examples

```csharp
// Called: sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
[Test]
        public void Method_AccessCacheOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            for (int i = 0; i < 100000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 1048575, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);
            int[] argbs = new int[]
            {
                //0xFFF8696B, 0xFFF98570, 0xFFFBA276, 0xFFFCBF7B, 0xFFFEDC81, 0xFFEDE582, 0xFFCADB80, 0xFFA8D17E, 0xFF85C77C, 0xFF63BE7B,
                -497301, -424592, -286090, -213125, -74623, -1186430, -3482752, -5713538, -8009860, -10240389,
            };

            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            TimePerformance monitor = new TimePerformance(70);
            monitor.StartPerfTest();
            Random random = new Random();
            for (int i = 0; i < 5000; i++)
            {
                int r = (int)(100000 * random.NextDouble());
                if (cells[r, 0].GetDisplayStyle(BorderType.None).ForegroundArgbColor != argbs[r % 10])
                {
                    Assert.Fail("A" + (r + 1) + " expected color should be "
                        + argbs[r % 10].ToString("X") + " but was "
                        + cells[r, 0].GetDisplayStyle().ForegroundArgbColor.ToString("X"));
                }
            }
            monitor.FinishPerfTest("Using access cache for conditional formattings with type of ColorScale");

            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


