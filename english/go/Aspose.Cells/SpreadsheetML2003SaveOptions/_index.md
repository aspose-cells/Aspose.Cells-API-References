---
title: SpreadsheetML2003SaveOptions Class 
linktitle: SpreadsheetML2003SaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'SpreadsheetML2003SaveOptions class. Encapsulates the object that represents spreadsheetml2003saveoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Represents the options for saving Excel 2003 spreadml file.

```go

type SpreadsheetML2003SaveOptions struct 

spreadsheetml2003saveoptions, _ := asposecells.NewSpreadsheetML2003SaveOptions()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[IsIndentedFormatting](./isindentedformatting/) | Causes child elements to be indented. | 
|[SetIsIndentedFormatting](./setisindentedformatting/) | Causes child elements to be indented. | 
|[GetLimitAsXls](./getlimitasxls/) | Limit as xls, the max row index is 65535 and the max column index is 255. | 
|[SetLimitAsXls](./setlimitasxls/) | Limit as xls, the max row index is 65535 and the max column index is 255. | 
|[GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | The default value is false, it means that column index  will be ignored if the cell is contiguous to the previous cell. | 
|[SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | The default value is false, it means that column index  will be ignored if the cell is contiguous to the previous cell. | 
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. | 
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. | 
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. | 
|[GetCachedFileFolder](./getcachedfilefolder/) | The cached file folder is used to store some large data. | 
|[SetCachedFileFolder](./setcachedfilefolder/) | The cached file folder is used to store some large data. | 
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
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
