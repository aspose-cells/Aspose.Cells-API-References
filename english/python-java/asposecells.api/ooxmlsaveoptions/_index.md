---
title: "OoxmlSaveOptions Class"
linktitle: "OoxmlSaveOptions"
articleTitle: "OoxmlSaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options of saving office open xml file."
type: docs
weight: 4090
url: /python-java/asposecells.api/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Represents the options of saving office open xml file.

## Constructors

| Name | Description |
| --- | --- |
| [OoxmlSaveOptions](#constructor) | Creates the options for saving office open xml file. |
| [OoxmlSaveOptions](#constructor) | Creates the options for saving office open xml file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [AsFlatOpc](#asflatopc) | boolean |  |
| [ExportCellName](#exportcellname) | boolean | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL S |
| [LightCellsDataProvider](#lightcellsdataprovider) | LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [UpdateZoom](#updatezoom) | boolean | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesT |
| [EnableZip64](#enablezip64) | boolean | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [EmbedOoxmlAsOleObject](#embedooxmlasoleobject) | boolean | Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject. |
| [CompressionType](#compressiontype) | int | Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant. T |
| [WpsCompatibility](#wpscompatibility) | boolean |  |
| [SaveFormat](#saveformat) | int | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [ClearData](#cleardata) | boolean | Make the workbook empty after saving the file. |
| [CachedFileFolder](#cachedfilefolder) | String | The cached file folder is used to store some large data. |
| [ValidateMergedAreas](#validatemergedareas) | boolean | Indicates whether validate merged cells before saving the file. The default value is false. |
| [MergeAreas](#mergeareas) | boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [CreateDirectory](#createdirectory) | boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [SortNames](#sortnames) | boolean | Indicates whether sorting defined names before saving file. |
| [SortExternalNames](#sortexternalnames) | boolean | Indicates whether sorting external defined names before saving file. |
| [RefreshChartCache](#refreshchartcache) | boolean | Indicates whether refreshing chart cache data |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

### OoxmlSaveOptions() (1 of 2) {#constructor}

Creates the options for saving office open xml file.

---

### OoxmlSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates the options for saving office open xml file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | A SaveFormat value. The file format. It should be one of following types: SaveFormat.XLSX , SaveFormat.XLTX , SaveFormat.XLAM , SaveFormat.XLSM or SaveFormat.XLTM , otherwise the saved format will be set as SaveFormat.XLSX automatically. |

### OoxmlSaveOptions.AsFlatOpc property {#asflatopc}

**Type:** boolean

### OoxmlSaveOptions.ExportCellName property {#exportcellname}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

**Type:** boolean

### OoxmlSaveOptions.LightCellsDataProvider property {#lightcellsdataprovider}

The data provider for saving workbook in light mode.

**Type:** LightCellsDataProvider

### OoxmlSaveOptions.UpdateZoom property {#updatezoom}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. The default value is false for performance.

**Type:** boolean

### OoxmlSaveOptions.EnableZip64 property {#enablezip64}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

**Type:** boolean

### OoxmlSaveOptions.EmbedOoxmlAsOleObject property {#embedooxmlasoleobject}

Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject.

**Type:** boolean

### OoxmlSaveOptions.CompressionType property {#compressiontype}

Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant. The default value is OoxmlCompressionType.Level2.

**Type:** int

### OoxmlSaveOptions.WpsCompatibility property {#wpscompatibility}

**Type:** boolean

### OoxmlSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### OoxmlSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### OoxmlSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### OoxmlSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### OoxmlSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### OoxmlSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### OoxmlSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### OoxmlSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### OoxmlSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### OoxmlSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### OoxmlSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### OoxmlSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
