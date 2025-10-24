##WebWorksheet.CreateSubtotal
WebWorksheet method. Creates subtotal in the sheet
## WebWorksheet.CreateSubtotal method
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
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
