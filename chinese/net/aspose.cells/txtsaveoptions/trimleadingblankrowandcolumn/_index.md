---
title: TrimLeadingBlankRowAndColumn
second_title: Aspose.Cells for .NET API 参考
description: 指示是否应该像 ms excel 那样修剪前导空白行和列 默认为真
type: docs
weight: 120
url: /zh/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

指示是否应该像 ms excel 那样修剪前导空白行和列。 默认为真。

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### 评论

与ms excel中的规则相同，如果行/列不被视为空白具有自定义样式 即使它不包含单元格数据。 使用 LightCells 模式保存时，此选项无效。 用户应通过执行[`LightCellsDataProvider`](../lightcellsdataprovider) 或指定P来控制输出范围:Aspose.Cells.TxtSaveOptions.ExportArea

### 也可以看看

* class [TxtSaveOptions](../../txtsaveoptions)
* 命名空间 [Aspose.Cells](../../txtsaveoptions)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
