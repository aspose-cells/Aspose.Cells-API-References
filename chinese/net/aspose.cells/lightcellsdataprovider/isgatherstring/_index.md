---
title: IsGatherString
second_title: Aspose.Cells for .NET API 参考
description: 检查cell的当前字符串值是否需要收集到全局池中
type: docs
weight: 10
url: /zh/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

检查cell的当前字符串值是否需要收集到全局池中。

```csharp
public bool IsGatherString()
```

### 返回值

如果需要将字符串值收集到生成文件的全局池中，则为 true。

### 评论

仅当此实现提供的单元格有许多重复的字符串值时，收集字符串值才会发挥优势。 在这种情况下，收集字符串将节省大量内存并生成更小的结果文件。 如果提供的单元格有很多字符串值由 LightCellsDataProvider 提供，但很少有相同的， 收集字符串将花费更多的内存和时间，并且对生成的文件没有优势。

### 也可以看看

* interface [LightCellsDataProvider](../../lightcellsdataprovider)
* 命名空间 [Aspose.Cells](../../lightcellsdataprovider)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
