##MainWeb.OnDoubleClickRowClientFunction
MainWeb property. Gets or sets the client side function to be called when a row is double clicked. The client function should be declared like this function MyOnRowDoubleClickrow  alertrow Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnDoubleClickRowClientFunction property
Gets or sets the client side function to be called when a row is double clicked. The client function should be declared like this: function MyOnRowDoubleClick(row) { alert(row); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnDoubleClickRowClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
