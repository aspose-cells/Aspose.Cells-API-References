---
title: StartCell
second_title: Aspose.Cells for .NET API 参考
description: 准备处理一个单元格
type: docs
weight: 30
url: /zh/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

准备处理一个单元格。

```csharp
public bool StartCell(int columnIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | Int32 | 要处理的单元格的列索引 |

### 返回值

是否需要处理此单元格。 false 忽略单元格并检查下一个单元格，直到到达当前行的单元格数据的末尾

### 评论

到达当前行中的现有单元格时将调用它。当前行是上次调用的行[`ProcessRow`](../processrow).

### 也可以看看

* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* 命名空间 [Aspose.Cells](../../lightcellsdatahandler)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
