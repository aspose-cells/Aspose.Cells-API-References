---
title: Class GridJsService
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.GridJsService class. Provides the basic operation apis used in controller actions
type: docs
url: /net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Provides the basic operation apis used in controller actions.

```csharp
public class GridJsService : IGridJsService
```

## Constructors

| Name | Description |
| --- | --- |
| [GridJsService](gridjsservice/)(IOptions&lt;GridJsOptions&gt;) | The default constructor for GridJsService |

## Properties

| Name | Description |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Represents the workbook settings. |

## Methods

| Name | Description |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/)(string, string, string, IFormFileCollection) | Applies the add image from local file operation. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Applies the add image from remote URL operation. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Applies the copy image operation. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Gets JSON string for the file by the specified unique id. . |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Gets JSON string for the Workbook by the specified unique id. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Write the JSON string for the file to the stream . |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Write the JSON string for the Workbook to the stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Write the JSON string for the file to the stream by the specified unique id. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Write the JSON string for the Workbook to the stream by the specified unique id. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Applies the download file operation |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Get file stream |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Get Stream of image. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Gets the image URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Gets the JSON string of the specified sheet in the file from the cache using the specified unique id. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Writes the JSON string of the specified sheet in the file from the cache using the specified unique id to the stream.. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Gets the byte array data of the embedded ole object . |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Translate all the string value to the target language in the worksheet |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Applies the update operation. |

### See Also

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


