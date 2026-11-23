---
title: "接口 IGridJsService"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.IGridJsService 接口。表示在控制器操作中使用的基本操作 API 接口"
type: docs
url: /zh/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

表示在控制器操作中使用的基本操作 API 接口。

```csharp
public interface IGridJsService : IDisposable
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | 执行从本地文件添加图像的操作，直接使用图像字节。 |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | 执行从本地文件添加图像的操作，使用上传的表单文件。 |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | 执行从远程 URL 添加图像的操作。 |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | 检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。 |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | 清除所有 JSON 缓存条目（内存和磁盘）。 |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | 清除属于指定唯一 ID 的所有 JSON 缓存条目。在带外修改源文件后调用此方法，以便下次请求重新生成 JSON。 |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | 执行复制图像的操作。 |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | 根据指定的唯一 ID 获取文件的 JSON 字符串。 |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | 根据指定的唯一 ID 获取工作簿的 JSON 字符串。 |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | 将工作簿的 JSON 字符串写入流中。 |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | 将工作簿的 JSON 字符串写入流中。 |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | 根据指定的唯一 ID 将文件的 JSON 字符串写入流中。 |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | 根据指定的唯一 ID 将工作簿的 JSON 字符串写入流中。 |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | 执行下载文件操作 |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | 获取文件流 |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | 获取导入文件的自定义警告回调。 |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | 获取图像的流。 |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | 获取图像 URL。 |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | 使用指定的唯一 ID，从缓存中获取文件中指定工作表的 JSON 字符串。 |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | 将使用指定唯一 ID 从缓存中获取的文件中指定工作表的 JSON 字符串写入流。 |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | 使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。 |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | 获取嵌入式 OLE 对象的字节数组数据。 |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | 设置导入文件的自定义警告回调。 |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | 执行更新操作。 |

### 另请参见

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


