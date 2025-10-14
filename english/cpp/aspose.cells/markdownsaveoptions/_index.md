---
title: Aspose::Cells::MarkdownSaveOptions class
linktitle: MarkdownSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::MarkdownSaveOptions class. Represents the save options for markdown in C++.'
type: docs
weight: 10300
url: /cpp/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class


Represents the save options for markdown.

```cpp
class MarkdownSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetAlignColumnPadding()](./getaligncolumnpadding/) | Indicates whether column alignment is enabled for generated [Markdown](../../aspose.cells.markdown/) tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default). |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCalculateFormula()](./getcalculateformula/) | Indicates whether to calculate formulas before saving markdown file. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEncoding()](./getencoding/) | Gets and sets the default encoding. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportHyperlinkAsReference()](./getexporthyperlinkasreference/) | Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false. |
| [GetExportImagesAsBase64()](./getexportimagesasbase64/) | Specifies whether images are saved in Base64 format to [Markdown](../../aspose.cells.markdown/). The default value is true. |
| [GetFormatStrategy()](./getformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
| [GetImageOptions()](./getimageoptions/) | Get the ImageOrPrintOptions object before exporting. |
| [GetLightCellsDataProvider()](./getlightcellsdataprovider/) | The Data provider to provide cells data for saving workbook in light mode. |
| [GetLineSeparator()](./getlineseparator/) | Gets and sets the line separator. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSheetSet()](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetSplitTablesByBlankRow()](./getsplittablesbyblankrow/) | Indicates whether blank rows in the worksheet should be treated as table separators when exporting to [Markdown](../../aspose.cells.markdown/). The default value is false. |
| [GetTableHeaderType()](./gettableheadertype/) | Gets and sets how set the header of the table. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [MarkdownSaveOptions()](./markdownsaveoptions/) | Creates options for saving markdown document. |
| [MarkdownSaveOptions(MarkdownSaveOptions_Impl* impl)](./markdownsaveoptions/) | Constructs from an implementation object. |
| [MarkdownSaveOptions(const MarkdownSaveOptions\& src)](./markdownsaveoptions/) | Copy constructor. |
| [MarkdownSaveOptions(const SaveOptions\& src)](./markdownsaveoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const MarkdownSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetAlignColumnPadding(char16_t value)](./setaligncolumnpadding/) | Indicates whether column alignment is enabled for generated [Markdown](../../aspose.cells.markdown/) tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default). |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCalculateFormula(bool value)](./setcalculateformula/) | Indicates whether to calculate formulas before saving markdown file. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEncoding(EncodingType value)](./setencoding/) | Gets and sets the default encoding. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportHyperlinkAsReference(bool value)](./setexporthyperlinkasreference/) | Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false. |
| [SetExportImagesAsBase64(bool value)](./setexportimagesasbase64/) | Specifies whether images are saved in Base64 format to [Markdown](../../aspose.cells.markdown/). The default value is true. |
| [SetFormatStrategy(CellValueFormatStrategy value)](./setformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
| [SetLightCellsDataProvider(LightCellsDataProvider* value)](./setlightcellsdataprovider/) | The Data provider to provide cells data for saving workbook in light mode. |
| [SetLineSeparator(const U16String\& value)](./setlineseparator/) | Gets and sets the line separator. |
| [SetLineSeparator(const char16_t* value)](./setlineseparator/) | Gets and sets the line separator. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSheetSet(const SheetSet\& value)](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetSplitTablesByBlankRow(bool value)](./setsplittablesbyblankrow/) | Indicates whether blank rows in the worksheet should be treated as table separators when exporting to [Markdown](../../aspose.cells.markdown/). The default value is false. |
| [SetTableHeaderType(MarkdownTableHeaderType value)](./settableheadertype/) | Gets and sets how set the header of the table. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~MarkdownSaveOptions()](./~markdownsaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
