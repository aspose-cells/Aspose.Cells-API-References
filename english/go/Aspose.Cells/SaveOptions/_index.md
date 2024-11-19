---
title: SaveOptions Class 
linktitle: SaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'SaveOptions class. Encapsulates the object that represents saveoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/saveoptions/
---

## SaveOptions class

Represents all save options

```go

type SaveOptions struct 

saveoptions, _ := asposecells.NewSaveOptions()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewSaveOptions](./newsaveoptions/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
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
