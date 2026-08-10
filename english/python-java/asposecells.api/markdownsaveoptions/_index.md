---
title: "MarkdownSaveOptions Class"
linktitle: "MarkdownSaveOptions"
articleTitle: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the save options for markdown."
type: docs
weight: 3570
url: /python-java/asposecells.api/markdownsaveoptions/
---

## MarkdownSaveOptions class

Represents the save options for markdown.

## Constructors

| Name | Description |
| --- | --- |
| [MarkdownSaveOptions](#constructor) | Creates options for saving markdown document |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Encoding](#encoding) | Encoding | Gets and sets the default encoding. |
| [FormatStrategy](#formatstrategy) | int | Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatS |
| [LightCellsDataProvider](#lightcellsdataprovider) | LightCellsDataProvider | The Data provider to provide cells data for saving workbook in light mode. |
| [LineSeparator](#lineseparator) | String | Gets and sets the line separator. |
| [TableHeaderType](#tableheadertype) | MarkdownTableHeaderType |  |
| [SheetSet](#sheetset) | SheetSet |  |
| [ImageOptions](#imageoptions) | ImageOrPrintOptions |  |
| [ExportImagesAsBase64](#exportimagesasbase64) | boolean |  |
| [StreamProvider](#streamprovider) | IStreamProvider |  |
| [CalculateFormula](#calculateformula) | boolean |  |
| [ExportHyperlinkAsReference](#exporthyperlinkasreference) | boolean |  |
| [AlignColumnPadding](#aligncolumnpadding) | char |  |
| [SplitTablesByBlankRow](#splittablesbyblankrow) | boolean |  |
| [OfficeMathOutputType](#officemathoutputtype) | int | The value of the property is HtmlOfficeMathOutputType integer constant. |
| [SaveFormat](#saveformat) | int | Gets the save file format. The value of the property is SaveFormat integer constant. |
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

### MarkdownSaveOptions() {#constructor}

Creates options for saving markdown document

### MarkdownSaveOptions.Encoding property {#encoding}

Gets and sets the default encoding.

**Type:** Encoding

### MarkdownSaveOptions.FormatStrategy property {#formatstrategy}

Gets and sets the format strategy when exporting the cell value as string. The value of the property is CellValueFormatStrategy integer constant.

**Type:** int

### MarkdownSaveOptions.LightCellsDataProvider property {#lightcellsdataprovider}

The Data provider to provide cells data for saving workbook in light mode.

**Type:** LightCellsDataProvider

### MarkdownSaveOptions.LineSeparator property {#lineseparator}

Gets and sets the line separator.

**Type:** String

### MarkdownSaveOptions.TableHeaderType property {#tableheadertype}

**Type:** MarkdownTableHeaderType

### MarkdownSaveOptions.SheetSet property {#sheetset}

**Type:** SheetSet

### MarkdownSaveOptions.ImageOptions property {#imageoptions}

**Type:** ImageOrPrintOptions

### MarkdownSaveOptions.ExportImagesAsBase64 property {#exportimagesasbase64}

**Type:** boolean

### MarkdownSaveOptions.StreamProvider property {#streamprovider}

**Type:** IStreamProvider

### MarkdownSaveOptions.CalculateFormula property {#calculateformula}

**Type:** boolean

### MarkdownSaveOptions.ExportHyperlinkAsReference property {#exporthyperlinkasreference}

**Type:** boolean

### MarkdownSaveOptions.AlignColumnPadding property {#aligncolumnpadding}

**Type:** char

### MarkdownSaveOptions.SplitTablesByBlankRow property {#splittablesbyblankrow}

**Type:** boolean

### MarkdownSaveOptions.OfficeMathOutputType property {#officemathoutputtype}

The value of the property is HtmlOfficeMathOutputType integer constant.

**Type:** int

### MarkdownSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### MarkdownSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### MarkdownSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### MarkdownSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### MarkdownSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### MarkdownSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### MarkdownSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### MarkdownSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### MarkdownSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### MarkdownSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### MarkdownSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### MarkdownSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### MarkdownSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
