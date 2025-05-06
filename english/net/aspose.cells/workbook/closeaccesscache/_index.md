---
title: Workbook.CloseAccessCache
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Closes the session that uses caches to access data
type: docs
url: /net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Closes the session that uses caches to access data.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |

### Examples

```csharp
// Called: wb.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
private void Method_AccessCacheOptions_(Workbook wb)
        {
            wb.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 128; i++)
            {
                for (int j = 0; j &lt; 16; j++)
                {
                    Cell cell = cells[i, j];
                    if (cell.StringValue[0] == &apos;D&apos;)
                    {
                        if (cell.GetDisplayStyle().Font.Size != 16)
                        {
                            StringBuilder sb = new StringBuilder();
                            sb.Append(cell.Name);
                            sb.Append(&quot;: should be formatted by conditional formatting but was not.\nPLEASE CHECK &quot;);
                            sb.Append(Constants.destPath);
                            sb.Append(&quot;J43108_res.xlsx&quot;);
                            wb.Save(Constants.destPath + &quot;J43108_res.xlsx&quot;);
                            Assert.Fail(sb.ToString());
                        }
                    }
                    else if (cell.GetDisplayStyle().Font.Size == 16)
                    {
                        StringBuilder sb = new StringBuilder();
                        sb.Append(cell.Name);
                        sb.Append(&quot;: should not be formatted by conditional formatting but was.\nPLEASE CHECK J43108_res.xlsx&quot;);
                        sb.Append(Constants.destPath);
                        sb.Append(&quot;J43108_res.xlsx&quot;);
                        Assert.Fail(sb.ToString());
                    }
                }
            }
            wb.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


