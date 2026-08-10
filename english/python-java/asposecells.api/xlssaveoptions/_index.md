---
title: "XlsSaveOptions Class"
linktitle: "XlsSaveOptions"
articleTitle: "XlsSaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the save options for the Excel 97-2003 file format: xls and xlt."
type: docs
weight: 7640
url: /python-java/asposecells.api/xlssaveoptions/
---

## XlsSaveOptions class

Represents the save options for the Excel 97-2003 file format: xls and xlt.

## Constructors

| Name | Description |
| --- | --- |
| [XlsSaveOptions](#constructor) | Creates options for saving Excel 97-2003 xls file. |
| [XlsSaveOptions](#constructor) | Creates options for saving Excel 97-2003 xls/xlt file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [LightCellsDataProvider](#lightcellsdataprovider) | LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [IsTemplate](#istemplate) | boolean | Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with  |
| [MatchColor](#matchcolor) | boolean | Indicates whether matching font color because there are 56 colors in the standard color palette. |
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

### XlsSaveOptions() (1 of 2) {#constructor}

Creates options for saving Excel 97-2003 xls file.

---

### XlsSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates options for saving Excel 97-2003 xls/xlt file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | A SaveFormat value. The file format. It should be SaveFormat.EXCEL_97_TO_2003 or SaveFormat.XLT , otherwise the saved format will be set as SaveFormat.EXCEL_97_TO_2003 automatically. |

### XlsSaveOptions.LightCellsDataProvider property {#lightcellsdataprovider}

The data provider for saving workbook in light mode.

**Type:** LightCellsDataProvider

### XlsSaveOptions.IsTemplate property {#istemplate}

Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with corresponding save format(xlt for true and xls for false). This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### XlsSaveOptions.MatchColor property {#matchcolor}

Indicates whether matching font color because there are 56 colors in the standard color palette.

**Type:** boolean

### XlsSaveOptions.WpsCompatibility property {#wpscompatibility}

**Type:** boolean

### XlsSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### XlsSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### XlsSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### XlsSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### XlsSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### XlsSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### XlsSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### XlsSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### XlsSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### XlsSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### XlsSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### XlsSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
