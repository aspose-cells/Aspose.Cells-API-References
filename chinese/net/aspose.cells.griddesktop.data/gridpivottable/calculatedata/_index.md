---
title: CalculateData
second_title: Aspose.Cells for .NET API 参考
description: 将数据透视表的数据计算到单元格
type: docs
weight: 20
url: /zh/net/aspose.cells.griddesktop.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

将数据透视表的数据计算到单元格。

```csharp
public void CalculateData()
```

### 评论

如果不调用该方法，枢轴范围内的Cell.Value无法返回正确的结果。 该方法使用内部枢轴缓存计算数据，而不是原始数据源。 所以如果数据源发生变化，请调用RefreshData () 方法优先。

### 也可以看看

* class [GridPivotTable](../../gridpivottable)
* 命名空间 [Aspose.Cells.GridDesktop.Data](../../gridpivottable)
* 部件 [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
