##Interface IGridJsService
Aspose.Cells.GridJs.IGridJsService interface. Reprensents the basic operation apis interface used in controller actions
## IGridJsService interface
Reprensents the basic operation apis interface used in controller actions.
```csharp
public interface IGridJsService
```
## Methods
| Name | Description |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/)(string, string, string, IFormFileCollection) |  |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) |  |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Applies the copy image operation. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Gets JSON string for the file by the specified unique id. . |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Gets JSON string for the Workbook by the specified unique id. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Write the JSON string for the Workbook to the stream |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Write the JSON string for the Workbook to the stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Write the JSON string for the file to the stream by the specified unique id. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Write the JSON string for the Workbook to the stream by the specified unique id. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Applies the download file operation |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Get file stream |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Get Stream of image. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Gets the image URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Gets the JSON string of the specified sheet in the file from the cache using the specified unique id. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Writes the JSON string of the specified sheet in the file from the cache using the specified unique id to the stream.. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Gets the byte array data of the embedded ole object . |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Applies the update operation. |
### See Also
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)
