---
title: "SvgSaveOptions Class"
linktitle: "SvgSaveOptions"
articleTitle: "SvgSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents Svg save options."
type: docs
weight: 6480
url: /php/aspose.cells/svgsaveoptions/
---

## SvgSaveOptions class

Represents Svg save options. For advanced usage, please use WorkbookRender or SheetRender .

## Constructors

| Name | Description |
| --- | --- |
| [SvgSaveOptions](#constructor) | Creates the options for saving svg file. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. T |
| [SvgSaveOptions](#constructor) | Creates the options for saving svg file. NOTE: This constructor is now obsolete. Instead, please use SvgSaveOptions() co |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [SheetIndex](#sheetindex) | Number | Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This  |
| [ImageOrPrintOptions](#imageorprintoptions) | ImageOrPrintOptions | Additional image creation options. For advanced usage, please use WorkbookRender or SheetRender . |
| [StreamProvider](#streamprovider) | IStreamProvider | Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more  |
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

### SvgSaveOptions() (1 of 2) {#constructor}

Creates the options for saving svg file. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

---

### SvgSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates the options for saving svg file. NOTE: This constructor is now obsolete. Instead, please use SvgSaveOptions() constructor. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The file format. It must be svg. |

### SvgSaveOptions.SheetIndex property {#sheetindex}

Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### SvgSaveOptions.ImageOrPrintOptions property {#imageorprintoptions}

Additional image creation options. For advanced usage, please use WorkbookRender or SheetRender .

**Type:** ImageOrPrintOptions

### SvgSaveOptions.StreamProvider property {#streamprovider}

Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use WorkbookRender or SheetRender .

**Type:** IStreamProvider

### SvgSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### SvgSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### SvgSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### SvgSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### SvgSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### SvgSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### SvgSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### SvgSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### SvgSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### SvgSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### SvgSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### SvgSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
