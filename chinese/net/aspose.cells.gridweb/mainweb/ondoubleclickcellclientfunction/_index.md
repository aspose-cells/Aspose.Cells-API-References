---
title: OnDoubleClickCellClientFunction
second_title: Aspose.Cells for .NET API 参考
description: 获取或设置双击单元格时要调用的客户端函数 客户端函数应该这样声明ltbr /gt function MyOnDoubleClickCellcellltbr /gt ltbr /gt GridWeb1.setCellValueByCellcell testltbr /gt ltbr /gtltbr /gt注意您可以在客户端函数中使用this指针指向触发事件的网格控件
type: docs
weight: 630
url: /zh/net/aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/
---
## MainWeb.OnDoubleClickCellClientFunction property

获取或设置双击单元格时要调用的客户端函数。 客户端函数应该这样声明:&lt;br /&gt; function MyOnDoubleClickCell(cell)&lt;br /&gt; {&lt;br /&gt; GridWeb1.setCellValueByCell(cell, "test");&lt;br /&gt; }&lt;br /&gt;&lt;br /&gt;注意:您可以在客户端函数中使用“this”指针指向触发事件的网格控件。

```csharp
public string OnDoubleClickCellClientFunction { get; set; }
```

### 也可以看看

* class [MainWeb](../../mainweb)
* 命名空间 [Aspose.Cells.GridWeb](../../mainweb)
* 部件 [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
