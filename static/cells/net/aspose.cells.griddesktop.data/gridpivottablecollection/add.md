##GridPivotTableCollection.Add
GridPivotTableCollection method. Adds a new PivotTable cache to a PivotCaches collection
## Add(string, string, string) {#add_3}
Adds a new PivotTable cache to a PivotCaches collection.
```csharp
public int Add(string sourceData, string destCellName, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### See Also
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(Worksheet, GridCellArea, string, string) {#add}
Adds a new PivotTable cache to a PivotCaches collection.
```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName,
string tableName)
```
| Parameter | Description |
| --- | --- |
| sourceSheet | The source work sheet. |
| sourceArea | The area in the source worksheet. |
| destRow | The row of the cell in the upper-left corner of the PivotTable report's destination range. |
| destCol | The column of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### See Also
* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string, GridCellArea, int, int, string) {#add_1}
Adds a new PivotTable cache to a PivotCaches collection.
```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol,
string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| worksheetname | String | The name of the source worksheet. |
| sourceArea | GridCellArea | The area in the source worksheet. |
| destRow | Int32 | The row of the cell in the upper-left corner of the PivotTable report's destination range. |
| destCol | Int32 | The column of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### See Also
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string, GridCellArea, string, string) {#add_2}
Adds a new PivotTable cache to a PivotCaches collection.
```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| worksheetname | String | The name of the source worksheet. |
| sourceArea | GridCellArea | The area in the source worksheet. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### See Also
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
