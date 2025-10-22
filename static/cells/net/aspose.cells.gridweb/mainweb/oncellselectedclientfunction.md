##MainWeb.OnCellSelectedClientFunction
MainWeb property. Gets or sets the client side function to be called when a cell is selected. The client function should be declared like this function MyOnSelectCellcell  GridWeb1.setCellValueByCellcell test Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnCellSelectedClientFunction property
Gets or sets the client side function to be called when a cell is selected. The client function should be declared like this: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnCellSelectedClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
