##GridJsWorkbook.CopyImageOrShape
GridJsWorkbook method. Copys image or shape
## GridJsWorkbook.CopyImageOrShape method
Copys image or shape.
```csharp
public string CopyImageOrShape(string uid, string p)
```
| Parameter | Type | Description |
| --- | --- | --- |
| uid | String | The unique id for the file cache. |
| p | String | The JSON string for the operation which specify the cell location ,it contains the worksheet name,upper left row,upper left column for the image or shape，etc {name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true} |
### Return Value
The JSON string of the new copied image
### See Also
* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
