---
title: OoxmlSaveOptions Class 
linktitle: OoxmlSaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'OoxmlSaveOptions class. Encapsulates the object that represents ooxmlsaveoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Represents the options of saving office open xml file.

```go

type OoxmlSaveOptions struct 

ooxmlsaveoptions, _ := asposecells.NewOoxmlSaveOptions()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetExportCellName](./getexportcellname/) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file.If the output file may be accessed by SQL Server DTS, this value must be true.Setting the value to false will highly increase the performance and reduce the file size when creating large file.Default value is true. | 
|[SetExportCellName](./setexportcellname/) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file.If the output file may be accessed by SQL Server DTS, this value must be true.Setting the value to false will highly increase the performance and reduce the file size when creating large file.Default value is true. | 
|[GetUpdateZoom](./getupdatezoom/) | Indicates whether update scaling factor before saving the fileif the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. | 
|[SetUpdateZoom](./setupdatezoom/) | Indicates whether update scaling factor before saving the fileif the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. | 
|[GetEnableZip64](./getenablezip64/) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. | 
|[SetEnableZip64](./setenablezip64/) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. | 
|[GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | Indicates whether embedding Ooxml files of OleObject as ole object. | 
|[SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | Indicates whether embedding Ooxml files of OleObject as ole object. | 
|[GetCompressionType](./getcompressiontype/) | Gets and sets the compression type for ooxml file. | 
|[SetCompressionType](./setcompressiontype/) | Gets and sets the compression type for ooxml file. | 
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
