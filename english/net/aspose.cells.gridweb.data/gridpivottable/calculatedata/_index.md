---
title: CalculateData
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 20
url: /net/aspose.cells.gridweb.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

Calculates pivottable's data to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method caclulates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### See Also

* class [GridPivotTable](../../gridpivottable)
* namespace [Aspose.Cells.GridWeb.Data](../../gridpivottable)
* assembly [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->