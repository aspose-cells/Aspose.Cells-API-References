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
private void Workbook_Method_CloseAccessCache(Workbook wb)
        {
            wb.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 128; i++)
            {
                for (int j = 0; j < 16; j++)
                {
                    Cell cell = cells[i, j];
                    if (cell.StringValue[0] == 'D')
                    {
                        if (cell.GetDisplayStyle().Font.Size != 16)
                        {
                            StringBuilder sb = new StringBuilder();
                            sb.Append(cell.Name);
                            sb.Append(": should be formatted by conditional formatting but was not.\nPLEASE CHECK ");
                            sb.Append(Constants.destPath);
                            sb.Append("example.xlsx");
                            wb.Save(Constants.destPath + "example.xlsx");
                            Assert.Fail(sb.ToString());
                        }
                    }
                    else if (cell.GetDisplayStyle().Font.Size == 16)
                    {
                        StringBuilder sb = new StringBuilder();
                        sb.Append(cell.Name);
                        sb.Append("example.xlsx");
                        sb.Append(Constants.destPath);
                        sb.Append("example.xlsx");
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


