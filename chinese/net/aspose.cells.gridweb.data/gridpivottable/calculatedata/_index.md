---
title: CalculateData
second_title: Aspose.Cells for .NET API 参考
description: 将数据透视表的数据计算到单元格
type: docs
weight: 20
url: /zh/net/aspose.cells.gridweb.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

将数据透视表的数据计算到单元格。

```csharp
public void CalculateData()
```

### 评论

Cell.Value 如果未调用该方法，则数据透视范围内的值无法返回正确的结果. 此方法使用内部数据透视缓存计算数据，而不是原始数据源。 所以如果数据源发生变化，请先调用 RefreshData() 方法。

### 也可以看看

* class [GridPivotTable](../../gridpivottable)
* 命名空间 [Aspose.Cells.GridWeb.Data](../../gridpivottable)
* 部件 [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->