---
title: PclSaveOptions Class 
linktitle: PclSaveOptions
second_title: Aspose.Cells for Go API Reference
description: 'PclSaveOptions class. Encapsulates the object that represents pclsaveoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/pclsaveoptions/
---

## PclSaveOptions class

Represents the options for saving Pcl file.

```go

type PclSaveOptions struct 

pclsaveoptions, _ := asposecells.NewPclSaveOptions()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewPclSaveOptions](./newpclsaveoptions/) | Creates the options for saving pdf file. | 
|[NewPclSaveOptions_PclSaveOptions](./newpclsaveoptions_pclsaveoptions/) | Constructs from an implementation object. | 
|[NewPclSaveOptions_PaginatedSaveOptions](./newpclsaveoptions_paginatedsaveoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[AddPrinterFont](./addprinterfont/) | Adds information about font that is already added to the printer by manufacturer. | 
|[GetDefaultFont](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. | 
|[SetDefaultFont](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. | 
|[GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. | 
|[SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. | 
|[SetCheckFontCompatibility](./setcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. | 
|[GetCheckFontCompatibility](./getcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. | 
|[SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. | 
|[IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. | 
|[GetOnePagePerSheet](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. | 
|[SetOnePagePerSheet](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. | 
|[GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be ignored, and the other settings of pagesetupwill still take effect. | 
|[SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be ignored, and the other settings of pagesetupwill still take effect. | 
|[GetIgnoreError](./getignoreerror/) | Indicates if you need to hide the error while rendering.The error can be error in shape, image, chart rendering, etc. | 
|[SetIgnoreError](./setignoreerror/) | Indicates if you need to hide the error while rendering.The error can be error in shape, image, chart rendering, etc. | 
|[GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. | 
|[SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. | 
|[SetPageIndex](./setpageindex/) | Gets or sets the 0-based index of the first page to save. | 
|[GetPageIndex](./getpageindex/) | Gets or sets the 0-based index of the first page to save. | 
|[SetPageCount](./setpagecount/) | Gets or sets the number of pages to save. | 
|[GetPageCount](./getpagecount/) | Gets or sets the number of pages to save. | 
|[GetPrintingPageType](./getprintingpagetype/) | Indicates which pages will not be printed. | 
|[SetPrintingPageType](./setprintingpagetype/) | Indicates which pages will not be printed. | 
|[GetGridlineType](./getgridlinetype/) | Gets or sets gridline type. | 
|[SetGridlineType](./setgridlinetype/) | Gets or sets gridline type. | 
|[GetTextCrossType](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. | 
|[SetTextCrossType](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. | 
|[GetDefaultEditLanguage](./getdefaulteditlanguage/) | Gets or sets default edit language. | 
|[SetDefaultEditLanguage](./setdefaulteditlanguage/) | Gets or sets default edit language. | 
|[GetSheetSet](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: <see cref="Aspose.Cells.Rendering.SheetSet.Visible"/>. | 
|[SetSheetSet](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: <see cref="Aspose.Cells.Rendering.SheetSet.Visible"/>. | 
|[GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. | 
|[SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. | 
|[GetEmfRenderSetting](./getemfrendersetting/) | Setting for rendering Emf metafile. | 
|[SetEmfRenderSetting](./setemfrendersetting/) | Setting for rendering Emf metafile. | 
