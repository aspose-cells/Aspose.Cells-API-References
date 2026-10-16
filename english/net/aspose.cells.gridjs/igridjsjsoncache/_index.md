---
title: Interface IGridJsJsonCache
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.IGridJsJsonCache interface. JSON cache interface  customers implement specific storage and invalidation strategies
type: docs
url: /net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

JSON cache interface - customers implement specific storage and invalidation strategies

```csharp
public interface IGridJsJsonCache
```

## Methods

| Name | Description |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Clear all caches |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Generate a cache key. Customers can decide whether to include the uid based on business requirements. - If only the file name matters: ignore uid and use fileName only (recommended, allows sharing cache across same file). - If distinguishing files with the same name is required: use uid (strict mode). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Invalidate the specified cache entry. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Invalidate all cache entries containing the specified uid. This is useful when you don't know the exact fileName used for caching. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Write JSON into cache. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Attempt to retrieve JSON from cache. |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


