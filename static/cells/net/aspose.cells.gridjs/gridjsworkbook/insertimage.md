##GridJsWorkbook.InsertImage
GridJsWorkbook method. Inserts image in the worksheet from file stream or the URLeither the file stream or the URL shall be provided or Inserts shape when the p.type is one of AutoShapeType
## GridJsWorkbook.InsertImage method
Inserts image in the worksheet from file stream or the URL,(either the file stream or the URL shall be provided) or Inserts shape ,when the p.type is one of AutoShapeType
```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```
| Parameter | Type | Description |
| --- | --- | --- |
| uid | String | The unique id for the file cache |
| p | String | The JSON format string for the operation which specify the cell location ,the worksheet name,upper left row,upper left column for the image，etc {name:'sheet1',ri:1,ci:1} |
| s | Stream | The file stream of the image file |
| imageUrl | String | The URL of the image file |
### Return Value
The JSON format string of the inserted image
### See Also
* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
