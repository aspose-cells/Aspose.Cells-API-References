---
title: GridJsWorkbook
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 80
url: /net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

the main entry class for GridJs

```csharp
public class GridJsWorkbook
```

## Constructors

| Name | Description |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | Represents the workbook settings. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | Callback interface of warning. |

## Methods

| Name | Description |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | copy image or shape in the worksheet |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | return error message |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson)() | Get json from workbook |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson)(string) | Get json from workbook |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | Get json from workbook |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | get the json from cache by uid |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(Workbook) | Imports from Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(Stream, GridLoadFormat) | Imports from an excel file stream.must provide loadformat and can set GridJsWorkbook.CacheImp to implement stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string, string) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string, Workbook) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(Stream, GridLoadFormat, string) | Imports from an excel file stream.must provide loadformat and can set GridJsWorkbook.CacheImp to implement stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string, Stream, GridLoadFormat) | Imports from an excel file stream.must provide loadformat and can set GridJsWorkbook.CacheImp to implement stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string, string, string) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile)(string, Stream, GridLoadFormat, string) | Imports from an excel file stream.must provide loadformat and can set GridJsWorkbook.CacheImp to implement stream cache |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | Import file from json |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | insert image in the worksheet |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | Apply style update to the cache file |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | Saves the worksheets to the cache, save format is baseed on the file extension of filename . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile)(Stream) | Saves the worksheets to the sream,baseed on the origin file format . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile)(string) | Saves the worksheets to the file path,if the file has extension ,save format is baseed on the file extension . |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml)(Stream) | Saves the worksheets to the sream,the save format is html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml)(string) | Saves the worksheets to the file path,the save format is html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf)(Stream) | Saves the worksheets to the sream,the save format is pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf)(string) | Saves the worksheets to the file path,the save format is pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx)(Stream) | Saves the worksheets to the sream,the save format is xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx)(string) | Saves the worksheets to the file path,the save format is xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | set InterruptMonitor for load operation for workbook |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | set InterruptMonitor for save operation for workbook |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | Do update operation |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | Get GridLoadFormat by file extension |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | Get Stream of Image from workbook |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | Get the image URL |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | Generate the uid for the file |

## Fields

| Name | Description |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | Custom implemention for cache storage,If you want to store cache in stream way ,you need to set and implement it |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | Custom implemention for calculation engine ,If you want to do custom calculation, you need to set and implement it |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* assembly [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
