---
title: "SpreadsheetML2003SaveOptions Class"
linktitle: "SpreadsheetML2003SaveOptions"
articleTitle: "SpreadsheetML2003SaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options for saving Excel 2003 spreadml file."
type: docs
weight: 6360
url: /python-java/asposecells.api/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Represents the options for saving Excel 2003 spreadml file.

## Constructors

| Name | Description |
| --- | --- |
| [SpreadsheetML2003SaveOptions](#constructor) | Creates the options for saving Excel 2003 spreadml file. |
| [SpreadsheetML2003SaveOptions](#constructor) | Creates the options for saving Excel 2003 spreadml file. NOTE: This constructor is now obsolete. Instead, please use Spr |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsIndentedFormatting](#isindentedformatting) | boolean | Causes child elements to be indented. The default value is true. If the value is false, it will reduce the size of the x |
| [LimitAsXls](#limitasxls) | boolean | Limit as xls, the max row index is 65535 and the max column index is 255. |
| [ExportColumnIndexOfCell](#exportcolumnindexofcell) | boolean | The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell. |
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

### SpreadsheetML2003SaveOptions() (1 of 2) {#constructor}

Creates the options for saving Excel 2003 spreadml file.

---

### SpreadsheetML2003SaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates the options for saving Excel 2003 spreadml file. NOTE: This constructor is now obsolete. Instead, please use SpreadsheetML2003SaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | A SaveFormat value. The save format. |

### SpreadsheetML2003SaveOptions.IsIndentedFormatting property {#isindentedformatting}

Causes child elements to be indented. The default value is true. If the value is false, it will reduce the size of the xml file

**Type:** boolean

### SpreadsheetML2003SaveOptions.LimitAsXls property {#limitasxls}

Limit as xls, the max row index is 65535 and the max column index is 255.

**Type:** boolean

### SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property {#exportcolumnindexofcell}

The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell.

**Type:** boolean

### SpreadsheetML2003SaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### SpreadsheetML2003SaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### SpreadsheetML2003SaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### SpreadsheetML2003SaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### SpreadsheetML2003SaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### SpreadsheetML2003SaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### SpreadsheetML2003SaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### SpreadsheetML2003SaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### SpreadsheetML2003SaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### SpreadsheetML2003SaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### SpreadsheetML2003SaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### SpreadsheetML2003SaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
