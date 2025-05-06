---
title: Workbook.StartAccessCache
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Starts the session that uses caches to access data
type: docs
url: /net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Starts the session that uses caches to access data.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |

### Remarks

If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them.  After finishing the access to the data, [`CloseAccessCache`](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.

### Examples

```csharp
// Called: wb.StartAccessCache(AccessCacheOptions.All);
[Test]
        public void Method_AccessCacheOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            cfc[cfc.Add()].Add(CellArea.CreateCellArea(0, 0, 3, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            Cells cells = sheet.Cells;
            cells[0, 0].PutValue(&quot;a?c&quot;);
            cells[1, 0].PutValue(&quot;def&quot;);
            cells[2, 0].PutValue(&quot;g?i&quot;);
            cells[3, 0].PutValue(&quot;def&quot;);
            wb.StartAccessCache(AccessCacheOptions.All);
            for (int i = 0; i &lt; 4; i++)
            {
                Assert.AreEqual(i % 2 == 0 ? BackgroundType.None : BackgroundType.Solid,
                    cells[i, 0].GetDisplayStyle().Pattern, &quot;A&quot; + (i + 1));
            }
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


