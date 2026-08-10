---
title: "XmlSaveOptions Class"
linktitle: "XmlSaveOptions"
articleTitle: "XmlSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the options of saving the workbook as an xml file."
type: docs
weight: 7700
url: /php/aspose.cells/xmlsaveoptions/
---

## XmlSaveOptions class

Represents the options of saving the workbook as an xml file.

## Constructors

| Name | Description |
| --- | --- |
| [XmlSaveOptions](#constructor) | Creates options for saving xml file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [SheetIndexes](#sheetindexes) | int[] | Represents the indexes of exported sheets. |
| [ExportArea](#exportarea) | CellArea | Gets or sets the exporting range. |
| [HasHeaderRow](#hasheaderrow) | boolean | Indicates whether the range contains header row. |
| [XmlMapName](#xmlmapname) | String | Indicates whether exporting xml map in the file. |
| [SheetNameAsElementName](#sheetnameaselementname) | boolean | Indicates whether exporting sheet's name as the name of the element. |
| [DataAsAttribute](#dataasattribute) | boolean | Indicates whether exporting data as attributes of element. |
| [SaveFormat](#saveformat) | Number | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [ClearData](#cleardata) | boolean | Make the workbook empty after saving the file. |
| [CachedFileFolder](#cachedfilefolder) | String | The cached file folder is used to store some large data. |
| [ValidateMergedAreas](#validatemergedareas) | boolean | Indicates whether validate merged cells before saving the file. The default value is false. |
| [MergeAreas](#mergeareas) | boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [CreateDirectory](#createdirectory) | boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [SortNames](#sortnames) | boolean | Indicates whether sorting defined names before saving file. |
| [SortExternalNames](#sortexternalnames) | boolean | Indicates whether sorting external defined names before saving file. |
| [RefreshChartCache](#refreshchartcache) | boolean | Indicates whether refreshing chart cache data |
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

### XmlSaveOptions() {#constructor}

Creates options for saving xml file.

### XmlSaveOptions.SheetIndexes property {#sheetindexes}

Represents the indexes of exported sheets.

**Type:** int[]

### XmlSaveOptions.ExportArea property {#exportarea}

Gets or sets the exporting range.

**Type:** CellArea

### XmlSaveOptions.HasHeaderRow property {#hasheaderrow}

Indicates whether the range contains header row.

**Type:** boolean

### XmlSaveOptions.XmlMapName property {#xmlmapname}

Indicates whether exporting xml map in the file.

**Type:** String

### XmlSaveOptions.SheetNameAsElementName property {#sheetnameaselementname}

Indicates whether exporting sheet's name as the name of the element.

**Type:** boolean

### XmlSaveOptions.DataAsAttribute property {#dataasattribute}

Indicates whether exporting data as attributes of element.

**Type:** boolean

### XmlSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### XmlSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### XmlSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### XmlSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### XmlSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### XmlSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### XmlSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### XmlSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### XmlSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### XmlSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### XmlSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### XmlSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### XmlSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
