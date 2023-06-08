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

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


