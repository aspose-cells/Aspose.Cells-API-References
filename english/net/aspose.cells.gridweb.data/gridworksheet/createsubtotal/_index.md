---
title: GridWorksheet.CreateSubtotal
second_title: Aspose.Cells for .NET API Reference
description: GridWorksheet method. Creates subtotal in the sheet
type: docs
url: /net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

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

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

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

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


