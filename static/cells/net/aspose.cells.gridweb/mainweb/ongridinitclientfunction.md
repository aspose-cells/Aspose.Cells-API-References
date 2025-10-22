##MainWeb.OnGridInitClientFunction
MainWeb property. Gets or sets the client side function name to be called when the grid is initialized. The client function should be declared like this function MyOnGridInitgrid  alertThe grid is initialized   grid.id Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnGridInitClientFunction property
Gets or sets the client side function name to be called when the grid is initialized. The client function should be declared like this: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnGridInitClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
