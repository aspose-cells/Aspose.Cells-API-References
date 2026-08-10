---
title: "OdsSaveOptions Class"
linktitle: "OdsSaveOptions"
articleTitle: "OdsSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the options of saving ods file."
type: docs
weight: 4030
url: /php/aspose.cells/odssaveoptions/
---

## OdsSaveOptions class

Represents the options of saving ods file.

## Constructors

| Name | Description |
| --- | --- |
| [OdsSaveOptions](#constructor) | Creates the options of saving ods file. |
| [OdsSaveOptions](#constructor) | Creates the options of saving ods file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [GeneratorType](#generatortype) | Number | Gets and sets the generator of the ods file. The value of the property is OdsGeneratorType integer constant. |
| [IsStrictSchema11](#isstrictschema11) | boolean | Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. NOTE: This member is now obs |
| [OdfStrictVersion](#odfstrictversion) | Number | Gets and sets the ODF version. The value of the property is OpenDocumentFormatVersionType integer constant. |
| [IgnorePivotTables](#ignorepivottables) | boolean |  |
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

### OdsSaveOptions() (1 of 2) {#constructor}

Creates the options of saving ods file.

---

### OdsSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates the options of saving ods file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The file format. It should be SaveFormat.ODS , SaveFormat.OTS , SaveFormat.FODS or SaveFormat.SXC , otherwise the saved format will be set as SaveFormat.ODS automatically. |

### OdsSaveOptions.GeneratorType property {#generatortype}

Gets and sets the generator of the ods file. The value of the property is OdsGeneratorType integer constant.

**Type:** Number

### OdsSaveOptions.IsStrictSchema11 property {#isstrictschema11}

Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### OdsSaveOptions.OdfStrictVersion property {#odfstrictversion}

Gets and sets the ODF version. The value of the property is OpenDocumentFormatVersionType integer constant.

**Type:** Number

### OdsSaveOptions.IgnorePivotTables property {#ignorepivottables}

**Type:** boolean

### OdsSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### OdsSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### OdsSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### OdsSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### OdsSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### OdsSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### OdsSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### OdsSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### OdsSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### OdsSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### OdsSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### OdsSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
