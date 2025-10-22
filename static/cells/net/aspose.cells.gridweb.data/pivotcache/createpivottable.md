##PivotCache.CreatePivotTable
PivotCache method. Creates PivotTable report to a new Sheet
## CreatePivotTable() {#createpivottable}
Creates PivotTable report to a new Sheet.
```csharp
public PivotTable CreatePivotTable()
```
### Return Value
The PivotTable object
### Remarks
Calling this method will create a PivotTable object and a new worksheet. Then adds the PivotTable object to the last location of GridWeb.Worksheets.PivotTables. If You call the PivotTable.DataBind() method, the PivotTable report will be painted to the created worksheet.
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## CreatePivotTable(string) {#createpivottable_3}
Creates PivotTable report to a new Sheet. The name of the pivotTable object
```csharp
public PivotTable CreatePivotTable(string tableName)
```
### Return Value
The PivotTable object
### Remarks
Calling this method will create a PivotTable object and a new worksheet. Then adds the PivotTable object to the last location of GridWeb.Worksheets.PivotTables. If You call the PivotTable.DataBind() method, the PivotTable report will be painted to the created worksheet.
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}
Creates PivotTable report to the targetSheet.
```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| targetSheet | WebWorksheet | The sheet that the pivotTable report will paint to |
| targetCell | WebCell | The start cell that the pivotTable report will paint to |
### Return Value
The PivotTable object
### Remarks
Calling this method will create a PivotTable object Then adds the PivotTable object to the last location of GridWeb.Worksheets.PivotTables. If You call the PivotTable.DataBind() method, the PivotTable report will be painted to the targetSheet starting at the targetCell.
### See Also
* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}
Creates PivotTable report to the targetSheet.
```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| targetSheet | WebWorksheet | The sheet that the pivotTable report will paint to |
| targetCell | WebCell | The start cell that the pivotTable report will paint to |
| tableName | String | The name of the pivotTable object |
### Return Value
The PivotTable object
### Remarks
Calling this method will create a PivotTable object naming tableName Then adds the PivotTable object to the last location of GridWeb.Worksheets.PivotTables. If You call the PivotTable.DataBind() method, the PivotTable report will be painted to the targetSheet starting at the targetCell.
### See Also
* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
