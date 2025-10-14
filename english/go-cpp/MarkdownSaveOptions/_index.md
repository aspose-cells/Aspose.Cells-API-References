---
title: MarkdownSaveOptions Class 
linktitle: MarkdownSaveOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'MarkdownSaveOptions class. Encapsulates the object that represents markdownsaveoptions in Go.'
type: docs
weight: 200
url: /go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Represents the save options for markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Creates options for saving markdown document | 
|[NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetEncoding](./getencoding/) | Gets and sets the default encoding. | 
|[SetEncoding](./setencoding/) | Gets and sets the default encoding. | 
|[GetFormatStrategy](./getformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. | 
|[SetFormatStrategy](./setformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. | 
|[GetLineSeparator](./getlineseparator/) | Gets and sets the line separator. | 
|[SetLineSeparator](./setlineseparator/) | Gets and sets the line separator. | 
|[GetTableHeaderType](./gettableheadertype/) | Gets and sets how set the header of the table. | 
|[SetTableHeaderType](./settableheadertype/) | Gets and sets how set the header of the table. | 
|[GetSheetSet](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Active. | 
|[SetSheetSet](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Active. | 
|[GetImageOptions](./getimageoptions/) | Get the ImageOrPrintOptions object before exporting | 
|[GetExportImagesAsBase64](./getexportimagesasbase64/) | Specifies whether images are saved in Base64 format to Markdown.The default value is true. | 
|[SetExportImagesAsBase64](./setexportimagesasbase64/) | Specifies whether images are saved in Base64 format to Markdown.The default value is true. | 
|[GetCalculateFormula](./getcalculateformula/) | Indicates whether to calculate formulas before saving markdown file. | 
|[SetCalculateFormula](./setcalculateformula/) | Indicates whether to calculate formulas before saving markdown file. | 
|[GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Indicates whether to export hyperlink using reference definitions instead of inline format.The default value is false. | 
|[SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Indicates whether to export hyperlink using reference definitions instead of inline format.The default value is false. | 
|[GetAlignColumnPadding](./getaligncolumnpadding/) | Indicates whether column alignment is enabled for generated Markdown tables.When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces).Set to '\0' to disable column alignment (default). | 
|[SetAlignColumnPadding](./setaligncolumnpadding/) | Indicates whether column alignment is enabled for generated Markdown tables.When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces).Set to '\0' to disable column alignment (default). | 
|[GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown.The default value is false. | 
|[SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown.The default value is false. | 
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. | 
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. | 
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. | 
|[GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. | 
|[SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. | 
|[GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. | 
|[SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. | 
|[GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. | 
|[SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. | 
|[GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. | 
|[SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. | 
|[GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. | 
|[SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. | 
|[GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. | 
|[SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. | 
|[GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether refreshing chart cache data | 
|[SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether refreshing chart cache data | 
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. | 
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. | 
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. | 
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. | 
