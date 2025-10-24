##MainWeb.OnSubmitClientFunction
MainWeb property. Gets or sets the client function to be called before the control is submitted at client side. The client function should be declared like this function MyOnSubmitarg cancelEdit  return true The arg is the submit argument contains the command to be post to the server. The cancelEdit is boolean value indicates whether the control has discarded the user input before submit. The control will continue submitting if the function returns true. Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnSubmitClientFunction property
Gets or sets the client function to be called before the control is submitted at client side. The client function should be declared like this: function MyOnSubmit(arg, cancelEdit) { return true;} The arg is the submit argument, contains the command to be post to the server. The cancelEdit is boolean value indicates whether the control has discarded the user input before submit. The control will continue submitting if the function returns true. Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnSubmitClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
