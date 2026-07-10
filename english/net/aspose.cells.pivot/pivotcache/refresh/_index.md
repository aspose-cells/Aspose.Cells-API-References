---
title: PivotCache.Refresh
second_title: Aspose.Cells for .NET API Reference
description: PivotCache method. Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache
type: docs
url: /net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### Remarks

It's better that you can simply call [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file.

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```csharp
public PivotRefreshState Refresh()
```

### Remarks

If both table1 and table2 use this cache, the two table will calculated. It's better that you can simply call [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file.

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


