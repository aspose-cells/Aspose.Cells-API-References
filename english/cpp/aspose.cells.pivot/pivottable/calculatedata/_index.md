---
title: Aspose::Cells::Pivot::PivotTable::CalculateData method
linktitle: CalculateData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotTable::CalculateData method. Calculates data of pivottable to cells in C++.'
type: docs
weight: 15100
url: /cpp/aspose.cells.pivot/pivottable/calculatedata/
---
## PivotTable::CalculateData() method


Calculates data of pivottable to cells.

```cpp
void Aspose::Cells::Pivot::PivotTable::CalculateData()
```

## Remarks


This method only calculate data with the cached data in the [PivotCache](../../pivotcache/). So if you want to calcualte with latest data source, please use [PivotCache.Refresh()](../../pivotcache/refresh/) method to calculate. If only the setting of pivot table is changed, [PivotTable.CalculateData()](./) is enough. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotTable::CalculateData(const PivotTableCalculateOption\&) method


Calculates pivot table with options.

```cpp
Vector<PivotTable> Aspose::Cells::Pivot::PivotTable::CalculateData(const PivotTableCalculateOption &option)
```


| Parameter | Type | Description |
| --- | --- | --- |
| option | const PivotTableCalculateOption\& | The options for calculating the pivot table |

## ReturnValue

Returns all pivot tables which have been calculated. If PivotTableCalculateOption.RefreshData is true,all pivot tables based on same pivot cache will be calculated together.
## Remarks



If PivotTableCalculateOption.RefreshData is true, this method will refresh pivot cache from data source,then calculate all pivot tables based same pivot cache. Otherwise, only calculating with the cached data in the pivot cache. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../)
* Class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
