---
title: XlsSaveOptions Class 
linktitle: XlsSaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'XlsSaveOptions class. Encapsulates the object that represents xlssaveoptions in Go.'
type: docs
weight: 200
url: /go/xlssaveoptions/
---

## XlsSaveOptions class

Represents the save options for the Excel 97-2003 file format: xls and xlt.

```go

type XlsSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewXlsSaveOptions](./newxlssaveoptions/) | Creates options for saving Excel 97-2003 xls file. | 
|[NewXlsSaveOptions_SaveFormat](./newxlssaveoptions_saveformat/) | Creates options for saving Excel 97-2003 xls/xlt file. | 
|[NewXlsSaveOptions_SaveOptions](./newxlssaveoptions_saveoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetMatchColor](./getmatchcolor/) | Indicates whether matching font color because there are 56 colors in the standard color palette. | 
|[SetMatchColor](./setmatchcolor/) | Indicates whether matching font color because there are 56 colors in the standard color palette. | 
|[GetWpsCompatibility](./getwpscompatibility/) | Indicates whether to make the xls more compatible with WPS. | 
|[SetWpsCompatibility](./setwpscompatibility/) | Indicates whether to make the xls more compatible with WPS. | 
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
