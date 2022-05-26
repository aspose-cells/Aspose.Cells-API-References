---
title: AddCustomFilter
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 450
url: /net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## Worksheet.AddCustomFilter method (1 of 2)

Add custom filter for the specified row range from start row to end row.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startrow | Int32 | The startrow of the filter range |
| startcolumn | Int32 | The startcolumn of the filter range |
| critiras | Object[] | The critira array for the columns,each one apply to each column |
| filterOperatorTypes | GridFilterOperatorType[] | The filter operate type array for the columns,each one apply to each column |

### See Also

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype)
* class [Worksheet](../../worksheet)
* namespace [Aspose.Cells.GridDesktop](../../worksheet)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Worksheet.AddCustomFilter method (2 of 2)

Add custom filter for the specified row.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Remarks

The filter criteria string. notice we use , and ; as split char,so the cell value shall not contains with those split char below are the criteria string examples: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### See Also

* class [Worksheet](../../worksheet)
* namespace [Aspose.Cells.GridDesktop](../../worksheet)
* assembly [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->