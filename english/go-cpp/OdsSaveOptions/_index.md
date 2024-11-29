---
title: OdsSaveOptions Class 
linktitle: OdsSaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'OdsSaveOptions class. Encapsulates the object that represents odssaveoptions in Go.'
type: docs
weight: 200
url: /go/odssaveoptions/
---

## OdsSaveOptions class

Represents the options of saving ods file.

```go

type OdsSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewOdsSaveOptions](./newodssaveoptions/) | Creates the options of saving ods file. | 
|[NewOdsSaveOptions_SaveFormat](./newodssaveoptions_saveformat/) | Creates the options of saving ods file. | 
|[NewOdsSaveOptions_SaveOptions](./newodssaveoptions_saveoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetGeneratorType](./getgeneratortype/) | Gets and sets the generator of the ods file. | 
|[SetGeneratorType](./setgeneratortype/) | Gets and sets the generator of the ods file. | 
|[GetOdfStrictVersion](./getodfstrictversion/) | Gets and sets the ODF version. | 
|[SetOdfStrictVersion](./setodfstrictversion/) | Gets and sets the ODF version. | 
|[GetIgnorePivotTables](./getignorepivottables/) | Indicates whether saving pivot tables. | 
|[SetIgnorePivotTables](./setignorepivottables/) | Indicates whether saving pivot tables. | 
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
