---
title: CreateSubtotal
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 490
url: /net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## GridWorksheet.CreateSubtotal method (1 of 2)

Creates subtotal in the sheet.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | Int32 | The row index of the column name row. |
| dataRows | Int32 | The number of the data rows. |
| groupByColumnIndex | Int32 | The column index of the column to be grouped. |
| subtotalFunction | SubtotalFunction | The subtotal function type. |
| subtotalColumnIndexList | Int32[] | The column indexes to be subtotaled. |
| functionLabel | String | The label of subtotal function. |
| grandCellStyle | GridTableItemStyle | The style of the grand total line. |
| subtotalCellStyle | GridTableItemStyle | The style of the subtotal line. |
| numberType | NumberType | The number type of the subtotal result cells. |
| customString | String | The custome format string of the subtotal result cells. Can be null. |

### See Also

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle)
* enum [NumberType](../../numbertype)
* class [GridWorksheet](../../gridworksheet)
* namespace [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## GridWorksheet.CreateSubtotal method (2 of 2)

Creates subtotal in the sheet.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | Int32 | The row index of the column name row. |
| dataRows | Int32 | The number of the data rows. |
| groupByColumnIndex | Int32 | The column index of the column to be grouped. |
| subtotalFunction | SubtotalFunction | The subtotal function type. |
| subtotalColumnIndexList | Int32[] | The column indexes to be subtotaled. |

### See Also

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridWorksheet](../../gridworksheet)
* namespace [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* assembly [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->