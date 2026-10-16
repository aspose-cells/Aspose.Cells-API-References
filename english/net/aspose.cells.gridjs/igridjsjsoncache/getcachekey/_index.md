---
title: IGridJsJsonCache.GetCacheKey
second_title: Aspose.Cells for .NET API Reference
description: IGridJsJsonCache method. Generate a cache key. Customers can decide whether to include the uid based on business requirements.  If only the file name matters ignore uid and use fileName only recommended allows sharing cache across same file.  If distinguishing files with the same name is required use uid strict mode
type: docs
url: /net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Generate a cache key. Customers can decide whether to include the uid based on business requirements. - If only the file name matters: ignore uid and use fileName only (recommended, allows sharing cache across same file). - If distinguishing files with the same name is required: use uid (strict mode).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uid | String | Unique identifier of the file (may differ per load) |
| fileName | String | Original file name |

### Return Value

Cache key

### See Also

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


