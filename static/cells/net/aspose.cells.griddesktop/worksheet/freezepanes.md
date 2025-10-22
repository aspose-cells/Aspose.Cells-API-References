##Worksheet.FreezePanes
Worksheet method. Freezes panes at the specified cell in the worksheet
## FreezePanes(string, int, int) {#freezepanes_1}
Freezes panes at the specified cell in the worksheet.
```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## FreezePanes(int, int, int, int) {#freezepanes}
Freezes panes at the specified cell in the worksheet.
```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
The first two parameters specify the freezed position and the last two parameters specify the area freezed on the left top pane.
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
