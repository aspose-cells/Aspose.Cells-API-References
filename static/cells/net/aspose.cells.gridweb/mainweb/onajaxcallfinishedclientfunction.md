##MainWeb.OnAjaxCallFinishedClientFunction
MainWeb property. Gets or sets the client side function name to be called when ajaxcall finished. The client function should be declared like this function GridAjaxcallFinished  alertthis.id ajaxcall finished  Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnAjaxCallFinishedClientFunction property
Gets or sets the client side function name to be called when ajaxcall finished. The client function should be declared like this: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnAjaxCallFinishedClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
