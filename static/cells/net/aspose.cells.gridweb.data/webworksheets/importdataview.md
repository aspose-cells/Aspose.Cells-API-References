##WebWorksheets.ImportDataView
WebWorksheets method. Imports from a DataView. Creates a sheet with the DataViews table name automatically
## ImportDataView(DataView, TableItemStyle, TableItemStyle) {#importdataview}
Imports from a DataView. Creates a sheet with the DataView's table name automatically.
```csharp
public void ImportDataView(DataView dataView, TableItemStyle colHeaderStyle,
TableItemStyle dataStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object. |
| colHeaderStyle | TableItemStyle | Specifies the style of the dataview header bar. |
| dataStyle | TableItemStyle | Specifies the style of the data area. |
### See Also
* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebWorksheets](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## ImportDataView(DataView, TableItemStyle, TableItemStyle, string, int, int) {#importdataview_1}
Imports from a DataView to the specified sheet and position.
```csharp
public void ImportDataView(DataView dataView, TableItemStyle colHeaderStyle,
TableItemStyle dataStyle, string sheetName, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object. |
| colHeaderStyle | TableItemStyle | Specifies the style of the dataview header bar. |
| dataStyle | TableItemStyle | Specifies the style of the data area. |
| sheetName | String | Specifies the sheet name. If the sheet doesn't exist, it will be created for you. |
| row | Int32 | Specifies the import position. |
| column | Int32 | Specifies the import postion. |
### See Also
* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebWorksheets](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
