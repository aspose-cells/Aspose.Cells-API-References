---
title: "PivotCache.Refresh"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotCache 方法。刷新来自数据源的数据，并为所有使用此数据缓存作为数据源的透视表计算视图数据。"
type: docs
url: /zh/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表的视图计算数据。

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | PivotTableRefreshOption | 刷新透视表数据源的选项。 |

### 备注

您可以直接调用[`RefreshAll`](../../../aspose.cells/workbook/refreshall/)来刷新文件中的所有透视表和图表，这样更好。

### 另请参见

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表的视图计算数据。

```csharp
public PivotRefreshState Refresh()
```

### 备注

如果 table1 和 table2 都使用此缓存，则两个表将被计算。您可以直接调用[`RefreshAll`](../../../aspose.cells/workbook/refreshall/)来刷新文件中的所有透视表和图表，这样更好。

### 另请参见

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


