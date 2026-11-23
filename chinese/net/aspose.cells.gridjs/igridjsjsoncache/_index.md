---
title: "接口 IGridJsJsonCache"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.IGridJsJsonCache 接口。JSON 缓存接口，客户实现特定的存储和失效策略"
type: docs
url: /zh/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

JSON 缓存接口 - 客户实现特定的存储和失效策略

```csharp
public interface IGridJsJsonCache
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | 清除所有缓存 |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | 生成缓存键。客户可以根据业务需求决定是否包含 uid。- 如果仅关心文件名：忽略 uid，仅使用 fileName（推荐，允许在相同文件之间共享缓存）。- 如果需要区分同名文件：使用 uid（严格模式）。 |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | 使指定的缓存条目失效。 |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | 使所有包含指定 uid 的缓存条目失效。当您不知道用于缓存的确切 fileName 时，这很有用。 |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | 将 JSON 写入缓存。 |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | 尝试从缓存中检索 JSON。 |

### 另请参见

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


