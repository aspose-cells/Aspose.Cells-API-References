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

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


