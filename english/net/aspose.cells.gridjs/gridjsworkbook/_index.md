---
title: Class GridJsWorkbook
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.GridJsWorkbook class. Represents the main entry class for GridJs
type: docs
url: /net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Represents the main entry class for GridJs

```csharp
public class GridJsWorkbook
```

## Constructors

| Name | Description |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Represents the workbook settings. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Gets or sets warning callback for import file. |

## Methods

| Name | Description |
| --- | --- |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only. |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Copys image or shape. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Gets the error message string in JSON format. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Gets JSON string from memory data, the default filename in the JSON is: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Gets JSON string from memory data,set the output filename in the JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string) | Gets JSON string from memory data,set the output filename in the JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Gets the byte array data of the embedded ole object . |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Imports the excel file from the file path. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Imports the excel file from the Workbook object. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Imports the excel file from file stream with load format. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Imports the excel file from the file path. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Imports the excel file from the Workbook object. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Imports the excel file from file stream with load format and open password. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Imports the excel file from file stream. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Imports the excel file from file path and open password. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Imports the excel file from file stream with load format and open password. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Imports the excel file from JSON format string. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Inserts image in the worksheet from file stream or the URL,(either the file stream or the URL shall be provided) or Inserts shape ,when the p.type is one of AutoShapeType |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string) | Retrieve the JSON string from memory data,set the output filename in the JSON, and write it to the stream. |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Retrieve the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON,and write it to the stream. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Gets the JSON string of the specified sheet in the file from the cache using the specified unique id. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Retrieve the JSON string of the specified sheet in the file from the cache using the specified unique id, and write it to the stream. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Applies a batch update to the memory data. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Saves the memory data to the cache file with the specified filename and also set the open password, the save format is baseed on the file extension of the filename . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Saves the memory data to the sream, baseed on the origin file format. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Saves the memory data to the file path,if the file has extension ,save format is baseed on the file extension . |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Saves the memory data to the sream,the save format is html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Saves the memory data to the file path,the save format is html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Saves the memory data to the sream,the save format is pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Saves the memory data to the file path,the save format is pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Saves the memory data to the sream,the save format is xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Saves the memory data to the file path,the save format is xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Sets InterruptMonitor for load operation. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Sets InterruptMonitor for save operation. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Translate all the string value to the target language in the worksheet |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Applies the update operation. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Gets the load format by file extension |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string) | Get Stream of image. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Gets the image URL. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Generates a new unique id for the file cache using the given file name. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Set the base image get action URL from controller . |

## Fields

| Name | Description |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Custom implemention for cache storage,If you want to store cache in stream way ,you need to set and implement it. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Custom implemention for calculation engine ,If you want to do custom calculation, you need to set and implement it. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | const value for the type of the image |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Gets/Sets the update monitor to track update operation |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


