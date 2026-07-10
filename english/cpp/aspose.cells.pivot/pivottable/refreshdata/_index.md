---
title: Aspose::Cells::Pivot::PivotTable::RefreshData method
linktitle: RefreshData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotTable::RefreshData method. Refreshes data from it''s data source to pivot cache in C++.'
type: docs
weight: 15000
url: /cpp/aspose.cells.pivot/pivottable/refreshdata/
---
## PivotTable::RefreshData() method


Refreshes data from it's data source to pivot cache.


>Deprecated
>
>Use PivotCache.RefreshData() method instead. 
```cpp
PivotRefreshState Aspose::Cells::Pivot::PivotTable::RefreshData()
```

## Remarks


We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. And it's better that you can simply call [Workbook.RefreshAll()](../../../aspose.cells/workbook/refreshall/) to refresh and calculate all pivot tables in the file, not to refresh one by one. NOTE: This method is now obsolete. Instead, please use [PivotCache.Refresh()](../../pivotcache/refresh/) method and remove followed [PivotTable.CalculateData()](../calculatedata/) because this pivot table will be caclualted when refreshing [PivotCache](../../pivotcache/). This method will be removed 12 months later since June 2026. **Aspose** apologizes for any inconvenience you may have experienced. 


## See Also

* Enum [PivotRefreshState](../../pivotrefreshstate/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotTable::RefreshData(const PivotTableRefreshOption\&) method


Refreshes pivottable's data and setting from it's data source with options.


>Deprecated
>
>Use PivotCache.RefreshData() method instead. 
```cpp
PivotRefreshState Aspose::Cells::Pivot::PivotTable::RefreshData(const PivotTableRefreshOption &option)
```


| Parameter | Type | Description |
| --- | --- | --- |
| option | const PivotTableRefreshOption\& | The options for refreshing data source of pivot table. |
## Remarks



We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. And it's better that you can simply call [Workbook.RefreshAll()](../../../aspose.cells/workbook/refreshall/) to refresh and calculate all pivot tables in the file, not to refresh one by one. NOTE: This method is now obsolete. Instead, please use [PivotCache.Refresh()](../../pivotcache/refresh/) method and remove followed [PivotTable.CalculateData()](../calculatedata/) because this pivot table will be caclualted when refreshing [PivotCache](../../pivotcache/) This method will be removed 12 months later since June 2026. **Aspose** apologizes for any inconvenience you may have experienced. 


## See Also

* Enum [PivotRefreshState](../../pivotrefreshstate/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
