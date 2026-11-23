---
title: "类 GridJsService"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.GridJsService 类。提供在控制器操作中使用的基本操作 API。"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

提供在控制器操作中使用的基本操作 API。

```csharp
public class GridJsService : IGridJsService
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | 针对自行构建选项对象的主机（浏览器 WASM 主机以及任何非 DI 服务器设置）的 GridJsService 构造函数。 |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | GridJsService 的默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | 表示工作簿设置。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | 执行从本地文件添加图像的操作（文件字节来自 JS FormData 或任何主机）。 |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | 执行从本地文件添加图像的操作。 |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | 执行从远程 URL 添加图像的操作。 |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | 检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。 |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | 清除所有 JSON 缓存条目（内存和磁盘）。 |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | 清除属于指定唯一 ID 的所有 JSON 缓存条目。在带外修改源文件后调用此方法，以便下次请求重新生成 JSON。 |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | 执行复制图像的操作。 |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | 此方法仅适用于 Java，实现 DisposableBean 中的 destroy 方法，Spring 在请求完成后会自动调用，实际上它会调用 Dispose 方法。 |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | 根据指定的唯一 ID 获取文件的 JSON 字符串。 |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | 根据指定的唯一 ID 获取工作簿的 JSON 字符串。 |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | 将文件的 JSON 字符串写入流中。 |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | 将工作簿的 JSON 字符串写入流中。 |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | 根据指定的唯一 ID 将文件的 JSON 字符串写入流中。 |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | 根据指定的唯一 ID 将工作簿的 JSON 字符串写入流中。 |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | 执行下载文件操作 |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | 获取文件流 |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | 获取导入文件的自定义警告回调。 |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | 获取图像的流。 |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | 获取图像 URL。 |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | 使用指定的唯一 ID，从缓存中获取文件中指定工作表的 JSON 字符串。 |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | 将使用指定唯一 ID 从缓存中获取的文件中指定工作表的 JSON 字符串写入流。 |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | 使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。 |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | 获取嵌入式 OLE 对象的字节数组数据。 |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | 设置导入文件的自定义警告回调。 |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | 将工作表中的所有字符串值翻译为目标语言 |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | 执行更新操作。 |

### 另请参见

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


