---
title: JsonSaveOptions Class 
linktitle: JsonSaveOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'JsonSaveOptions class. Encapsulates the object that represents jsonsaveoptions in Go.'
type: docs
weight: 200
url: /go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Represents the options of saving the workbook as a JSON file.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewJsonSaveOptions](./newjsonsaveoptions/) | Creates options for saving json file. | 
|[NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetExportStylePool](./getexportstylepool/) | Indicates whether to export styles collectively or individually to each cell. | 
|[SetExportStylePool](./setexportstylepool/) | Indicates whether to export styles collectively or individually to each cell. | 
|[GetExportHyperlinkType](./getexporthyperlinktype/) | Represents the type of exporting hyperlink to json. | 
|[SetExportHyperlinkType](./setexporthyperlinktype/) | Represents the type of exporting hyperlink to json. | 
|[GetSkipEmptyRows](./getskipemptyrows/) | Indicates whether skipping emtpy rows. | 
|[SetSkipEmptyRows](./setskipemptyrows/) | Indicates whether skipping emtpy rows. | 
|[GetSheetIndexes](./getsheetindexes/) | Represents the indexes of exported sheets. | 
|[SetSheetIndexes](./setsheetindexes/) | Represents the indexes of exported sheets. | 
|[GetSchemas](./getschemas/) | The original json schema of each worksheet. | 
|[SetSchemas](./setschemas/) | The original json schema of each worksheet. | 
|[GetExportArea](./getexportarea/) | Gets or sets the exporting range. | 
|[SetExportArea](./setexportarea/) | Gets or sets the exporting range. | 
|[GetHasHeaderRow](./gethasheaderrow/) | Indicates whether the range contains header row. | 
|[SetHasHeaderRow](./sethasheaderrow/) | Indicates whether the range contains header row. | 
|[GetExportAsString](./getexportasstring/) | Exports the string value of the cells to json. | 
|[SetExportAsString](./setexportasstring/) | Exports the string value of the cells to json. | 
|[GetIndent](./getindent/) | Indicates the indent. | 
|[SetIndent](./setindent/) | Indicates the indent. | 
|[GetExportNestedStructure](./getexportnestedstructure/) | Exported as parent-child hierarchy Json structure. | 
|[SetExportNestedStructure](./setexportnestedstructure/) | Exported as parent-child hierarchy Json structure. | 
|[GetExportEmptyCells](./getexportemptycells/) | Indicates whether exporting empty cells as null. | 
|[SetExportEmptyCells](./setexportemptycells/) | Indicates whether exporting empty cells as null. | 
|[GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. | 
|[SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. | 
|[GetToExcelStruct](./gettoexcelstruct/) | Indicates whether converting to json struct of the Excel file. | 
|[SetToExcelStruct](./settoexcelstruct/) | Indicates whether converting to json struct of the Excel file. | 
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. | 
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. | 
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. | 
|[GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. | 
|[SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. | 
|[GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. | 
|[SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. | 
|[GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. | 
|[SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. | 
|[GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. | 
|[SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. | 
|[GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. | 
|[SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. | 
|[GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. | 
|[SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. | 
|[GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether refreshing chart cache data | 
|[SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether refreshing chart cache data | 
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. | 
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. | 
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
