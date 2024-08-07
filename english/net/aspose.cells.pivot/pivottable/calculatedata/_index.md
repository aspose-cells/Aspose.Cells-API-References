---
title: PivotTable.CalculateData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables data to cells
type: docs
url: /net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata}

Calculates pivottable's data to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata_1}

Calculating pivot tables with options

```csharp
public void CalculateData(PivotTableCalculateOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption |  |

### See Also

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


