##GridJsWorkbook.JsonToStreamByUid
GridJsWorkbook method. Retrieve the JSON string of the file from the cache using the specified unique idset the output filename in the JSONand write it to the stream
## GridJsWorkbook.JsonToStreamByUid method
Retrieve the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON,and write it to the stream.
```csharp
public bool JsonToStreamByUid(Stream stream, string uid, string filename)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream that will be written |
| uid | String | The unique id for the file cache. |
| filename | String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |
### See Also
* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
