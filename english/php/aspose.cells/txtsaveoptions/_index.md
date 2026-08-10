---
title: "TxtSaveOptions Class"
linktitle: "TxtSaveOptions"
articleTitle: "TxtSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the save options for csv/tab delimited/other text format."
type: docs
weight: 7170
url: /php/aspose.cells/txtsaveoptions/
---

## TxtSaveOptions class

Represents the save options for csv/tab delimited/other text format.

## Constructors

| Name | Description |
| --- | --- |
| [TxtSaveOptions](#constructor) | Creates text file save options. |
| [TxtSaveOptions](#constructor) | Creates text file save options. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Separator](#separator) | char | Gets and sets char Delimiter of text file. |
| [SeparatorString](#separatorstring) | String | Gets and sets a string value as separator. |
| [Encoding](#encoding) | Encoding | Gets and sets the default encoding. |
| [AlwaysQuoted](#alwaysquoted) | boolean | Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will on |
| [QuoteType](#quotetype) | Number | Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer const |
| [FormatStrategy](#formatstrategy) | Number | Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatS |
| [LightCellsDataProvider](#lightcellsdataprovider) | LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [TrimLeadingBlankRowAndColumn](#trimleadingblankrowandcolumn) | boolean | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with t |
| [TrimTailingBlankCells](#trimtailingblankcells) | boolean | Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode a |
| [KeepSeparatorsForBlankRow](#keepseparatorsforblankrow) | boolean | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank  |
| [ExportArea](#exportarea) | CellArea | The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no e |
| [ExportQuotePrefix](#exportquoteprefix) | boolean | Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is tr |
| [ExportAllSheets](#exportallsheets) | boolean | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel |
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

### TxtSaveOptions() (1 of 2) {#constructor}

Creates text file save options.

---

### TxtSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates text file save options.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The file format. It should be SaveFormat.CSV or SaveFormat.TSV , otherwise the saved format will be set as SaveFormat.CSV automatically. |

### TxtSaveOptions.Separator property {#separator}

Gets and sets char Delimiter of text file.

**Type:** char

### TxtSaveOptions.SeparatorString property {#separatorstring}

Gets and sets a string value as separator.

**Type:** String

### TxtSaveOptions.Encoding property {#encoding}

Gets and sets the default encoding.

**Type:** Encoding

### TxtSaveOptions.AlwaysQuoted property {#alwaysquoted}

Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false. NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### TxtSaveOptions.QuoteType property {#quotetype}

Gets or sets how to quote values in the exported text file. The value of the property is TxtValueQuoteType integer constant.

**Type:** Number

### TxtSaveOptions.FormatStrategy property {#formatstrategy}

Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatStrategy integer constant.

**Type:** Number

### TxtSaveOptions.LightCellsDataProvider property {#lightcellsdataprovider}

The data provider for saving workbook in light mode.

**Type:** LightCellsDataProvider

### TxtSaveOptions.TrimLeadingBlankRowAndColumn property {#trimleadingblankrowandcolumn}

Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of LightCellsDataProvider or by speicifing ExportArea

**Type:** boolean

### TxtSaveOptions.TrimTailingBlankCells property {#trimtailingblankcells}

Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode and the ExportArea has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation LightCellsDataProvider

**Type:** boolean

### TxtSaveOptions.KeepSeparatorsForBlankRow property {#keepseparatorsforblankrow}

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

**Type:** boolean

### TxtSaveOptions.ExportArea property {#exportarea}

The range of cells to be exported. If the exported area has been specified, TrimLeadingBlankRowAndColumn will takes no effect.

**Type:** CellArea

### TxtSaveOptions.ExportQuotePrefix property {#exportquoteprefix}

Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is true for it. Default is false.

**Type:** boolean

### TxtSaveOptions.ExportAllSheets property {#exportallsheets}

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. The defult value is false.

**Type:** boolean

### TxtSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### TxtSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### TxtSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### TxtSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### TxtSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### TxtSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### TxtSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### TxtSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### TxtSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### TxtSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### TxtSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### TxtSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
