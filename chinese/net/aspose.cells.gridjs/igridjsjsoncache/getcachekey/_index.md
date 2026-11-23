---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "IGridJsJsonCache 方法。生成缓存键。客户可以根据业务需求决定是否包含 uid。如果仅文件名重要，则忽略 uid，仅使用 fileName（推荐），允许在相同文件之间共享缓存。如果需要区分同名文件，则使用 uid 严格模式。"
type: docs
url: /zh/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

生成缓存键。客户可以根据业务需求决定是否包含 uid。- 如果仅关心文件名：忽略 uid，仅使用 fileName（推荐，允许在相同文件之间共享缓存）。- 如果需要区分同名文件：使用 uid（严格模式）。

```csharp
public string GetCacheKey(string uid, string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | String | 文件的唯一标识符（可能因加载而不同） |
| fileName | String | 原始文件名 |

### 返回值

缓存键

### 另请参见

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


