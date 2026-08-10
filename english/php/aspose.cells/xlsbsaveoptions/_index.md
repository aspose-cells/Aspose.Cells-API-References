---
title: "XlsbSaveOptions Class"
linktitle: "XlsbSaveOptions"
articleTitle: "XlsbSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the options for saving xlsb file."
type: docs
weight: 7650
url: /php/aspose.cells/xlsbsaveoptions/
---

## XlsbSaveOptions class

Represents the options for saving xlsb file.

## Constructors

| Name | Description |
| --- | --- |
| [XlsbSaveOptions](#constructor) | Creates xlsb file save options. |
| [XlsbSaveOptions](#constructor) | Creates xlsb file save options. NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructo |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CompressionType](#compressiontype) | Number | Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant. T |
| [ExportAllColumnIndexes](#exportallcolumnindexes) | boolean | Indicates whether exporting all column indexes for cells. The default value is true. |
| [LightCellsDataProvider](#lightcellsdataprovider) | LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [SaveFormat](#saveformat) | Number | Gets the save file format. The value of the property is SaveFormat integer constant. |
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

### XlsbSaveOptions() (1 of 2) {#constructor}

Creates xlsb file save options.

---

### XlsbSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates xlsb file save options. NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The save format . It must be xlsb. |

### XlsbSaveOptions.CompressionType property {#compressiontype}

Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant. The default value is OoxmlCompressionType.Level6.

**Type:** Number

### XlsbSaveOptions.ExportAllColumnIndexes property {#exportallcolumnindexes}

Indicates whether exporting all column indexes for cells. The default value is true.

**Type:** boolean

### XlsbSaveOptions.LightCellsDataProvider property {#lightcellsdataprovider}

The data provider for saving workbook in light mode.

**Type:** LightCellsDataProvider

### XlsbSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### XlsbSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### XlsbSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### XlsbSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### XlsbSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### XlsbSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### XlsbSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### XlsbSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### XlsbSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### XlsbSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### XlsbSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### XlsbSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
