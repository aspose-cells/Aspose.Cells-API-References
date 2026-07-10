---
title: Aspose::Cells::Pivot::PivotCache::Refresh method
linktitle: Refresh
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotCache::Refresh method. Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells.pivot/pivotcache/refresh/
---
## PivotCache::Refresh(const PivotTableRefreshOption\&) method


Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```cpp
PivotRefreshState Aspose::Cells::Pivot::PivotCache::Refresh(const PivotTableRefreshOption &option)
```


| Parameter | Type | Description |
| --- | --- | --- |
| option | const PivotTableRefreshOption\& | The options for refreshing data source of pivot table. |
## Remarks



It's better that you can simply call [Workbook.RefreshAll()](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file. 
## See Also

* Enum [PivotRefreshState](../../pivotrefreshstate/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* Class [PivotCache](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotCache::Refresh() method


Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```cpp
PivotRefreshState Aspose::Cells::Pivot::PivotCache::Refresh()
```

## Remarks


If both table1 and table2 use this cache, the two table will calculated. It's better that you can simply call [Workbook.RefreshAll()](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file. 
## See Also

* Enum [PivotRefreshState](../../pivotrefreshstate/)
* Class [PivotCache](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
