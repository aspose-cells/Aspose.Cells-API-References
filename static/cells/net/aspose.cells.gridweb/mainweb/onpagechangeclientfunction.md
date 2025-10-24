##MainWeb.OnPageChangeClientFunction
MainWeb property. Gets or sets the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this function MyOnPageChangeindex  console.logcurrent page isindex Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnPageChangeClientFunction property
Gets or sets the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this: function MyOnPageChange(index) { console.log("current page is:"+index); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnPageChangeClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
