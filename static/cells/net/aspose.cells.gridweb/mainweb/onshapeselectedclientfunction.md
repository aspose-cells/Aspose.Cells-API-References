##MainWeb.OnShapeSelectedClientFunction
MainWeb property. Gets or sets the client side function to be called when a shape is selected. The client function should be declared like this function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnShapeSelectedClientFunction property
Gets or sets the client side function to be called when a shape is selected. The client function should be declared like this: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnShapeSelectedClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
