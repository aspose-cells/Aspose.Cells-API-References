---
title: "JsonSaveOptions Class"
linktitle: "JsonSaveOptions"
articleTitle: "JsonSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the options of saving the workbook as a json file."
type: docs
weight: 3200
url: /php/aspose.cells/jsonsaveoptions/
---

## JsonSaveOptions class

Represents the options of saving the workbook as a json file.

## Constructors

| Name | Description |
| --- | --- |
| [JsonSaveOptions](#constructor) | Creates options for saving json file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ExportStylePool](#exportstylepool) | boolean |  |
| [ExportHyperlinkType](#exporthyperlinktype) | Number | Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constan |
| [SkipEmptyRows](#skipemptyrows) | boolean | Indicates whether skipping emtpy rows. |
| [SheetIndexes](#sheetindexes) | int[] | Represents the indexes of exported sheets. |
| [Schemas](#schemas) | String[] |  |
| [ExportArea](#exportarea) | CellArea | Gets or sets the exporting range. |
| [HasHeaderRow](#hasheaderrow) | boolean | Indicates whether the range contains header row. |
| [ExportAsString](#exportasstring) | boolean | Exports the string value of the cells to json. |
| [Indent](#indent) | String | Indicates the indent. If the indent is null or empty, the exported json is not formatted. |
| [ExportNestedStructure](#exportnestedstructure) | boolean | Exported as parent-child hierarchy Json structure. |
| [ExportEmptyCells](#exportemptycells) | boolean | Indicates whether exporting empty cells as null. |
| [AlwaysExportAsJsonObject](#alwaysexportasjsonobject) | boolean | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [ToExcelStruct](#toexcelstruct) | boolean | Indicates whether converting to json struct of the Excel file. Only for converting range to JSON. |
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

### JsonSaveOptions() {#constructor}

Creates options for saving json file.

### JsonSaveOptions.ExportStylePool property {#exportstylepool}

**Type:** boolean

### JsonSaveOptions.ExportHyperlinkType property {#exporthyperlinktype}

Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constant. The default value is JsonExportHyperlinkType.DISPLAY_STRING ;

**Type:** Number

### JsonSaveOptions.SkipEmptyRows property {#skipemptyrows}

Indicates whether skipping emtpy rows.

**Type:** boolean

### JsonSaveOptions.SheetIndexes property {#sheetindexes}

Represents the indexes of exported sheets.

**Type:** int[]

### JsonSaveOptions.Schemas property {#schemas}

**Type:** String[]

### JsonSaveOptions.ExportArea property {#exportarea}

Gets or sets the exporting range.

**Type:** CellArea

### JsonSaveOptions.HasHeaderRow property {#hasheaderrow}

Indicates whether the range contains header row.

**Type:** boolean

### JsonSaveOptions.ExportAsString property {#exportasstring}

Exports the string value of the cells to json.

**Type:** boolean

### JsonSaveOptions.Indent property {#indent}

Indicates the indent. If the indent is null or empty, the exported json is not formatted.

**Type:** String

### JsonSaveOptions.ExportNestedStructure property {#exportnestedstructure}

Exported as parent-child hierarchy Json structure.

**Type:** boolean

### JsonSaveOptions.ExportEmptyCells property {#exportemptycells}

Indicates whether exporting empty cells as null.

**Type:** boolean

### JsonSaveOptions.AlwaysExportAsJsonObject property {#alwaysexportasjsonobject}

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

**Type:** boolean

### JsonSaveOptions.ToExcelStruct property {#toexcelstruct}

Indicates whether converting to json struct of the Excel file. Only for converting range to JSON.

**Type:** boolean

### JsonSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### JsonSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### JsonSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### JsonSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### JsonSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### JsonSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### JsonSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### JsonSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### JsonSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### JsonSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### JsonSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### JsonSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### JsonSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
