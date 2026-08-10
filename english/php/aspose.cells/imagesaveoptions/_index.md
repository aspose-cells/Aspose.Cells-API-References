---
title: "ImageSaveOptions Class"
linktitle: "ImageSaveOptions"
articleTitle: "ImageSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents image save options."
type: docs
weight: 3110
url: /php/aspose.cells/imagesaveoptions/
---

## ImageSaveOptions class

Represents image save options. For advanced usage, please use WorkbookRender or SheetRender .

## Constructors

| Name | Description |
| --- | --- |
| [ImageSaveOptions](#constructor) | Creates the options for saving image file. The default type is Tiff. |
| [ImageSaveOptions](#constructor) | Creates the options for saving image file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
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

### ImageSaveOptions() (1 of 2) {#constructor}

Creates the options for saving image file. The default type is Tiff.

---

### ImageSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates the options for saving image file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The file format. It should be one of following types: SaveFormat.TIFF , SaveFormat.SVG , SaveFormat.BMP , SaveFormat.PNG , SaveFormat.JPG , SaveFormat.EMF or SaveFormat.GIF , otherwise the saved format will be set as SaveFormat.TIFF automatically. |

### ImageSaveOptions.ImageOrPrintOptions property {#imageorprintoptions}

Additional image creation options. For advanced usage, please use WorkbookRender or SheetRender .

**Type:** ImageOrPrintOptions

### ImageSaveOptions.StreamProvider property {#streamprovider}

Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use WorkbookRender or SheetRender .

**Type:** IStreamProvider

### ImageSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### ImageSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### ImageSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### ImageSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### ImageSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### ImageSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### ImageSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### ImageSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### ImageSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### ImageSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### ImageSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### ImageSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
