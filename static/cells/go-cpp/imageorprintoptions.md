##ImageOrPrintOptions Class
'ImageOrPrintOptions class. Encapsulates the object that represents imageorprintoptions in Go.'
## ImageOrPrintOptions class
Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.
```go
type ImageOrPrintOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewImageOrPrintOptions](./newimageorprintoptions/) | Ctor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[SetPrintWithStatusDialog](./setprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status.else no such dialog will show. |
|[GetPrintWithStatusDialog](./getprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status.else no such dialog will show. |
|[GetHorizontalResolution](./gethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
|[SetHorizontalResolution](./sethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
|[GetVerticalResolution](./getverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
|[SetVerticalResolution](./setverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
|[GetTiffCompression](./gettiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
|[SetTiffCompression](./settiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
|[GetTiffColorDepth](./gettiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
|[SetTiffColorDepth](./settiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
|[GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp formatwhen ImageType is Tiff and TiffCompression is equal to Ccitt3 or Ccitt4. |
|[SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp formatwhen ImageType is Tiff and TiffCompression is equal to Ccitt3 or Ccitt4. |
|[GetPrintingPage](./getprintingpage/) | Indicates which pages will not be printed. |
|[SetPrintingPage](./setprintingpage/) | Indicates which pages will not be printed. |
|[GetQuality](./getquality/) | Gets or sets a value determining the quality of the generated  imagesto apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
|[SetQuality](./setquality/) | Gets or sets a value determining the quality of the generated  imagesto apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
|[GetOnePagePerSheet](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[SetOnePagePerSheet](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
|[SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
|[GetOnlyArea](./getonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
|[SetOnlyArea](./setonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
|[GetTransparent](./gettransparent/) | Indicates if the background of generated image should be transparent. |
|[SetTransparent](./settransparent/) | Indicates if the background of generated image should be transparent. |
|[SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
|[IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
|[SetPageIndex](./setpageindex/) | Gets or sets the 0-based index of the first page to save. |
|[GetPageIndex](./getpageindex/) | Gets or sets the 0-based index of the first page to save. |
|[SetPageCount](./setpagecount/) | Gets or sets the number of pages to save. |
|[GetPageCount](./getpagecount/) | Gets or sets the number of pages to save. |
|[SetDesiredSize](./setdesiredsize/) | Sets desired width and height of image. |
|[IsOptimized](./isoptimized/) | Indicates whether to optimize the output elements. |
|[SetIsOptimized](./setisoptimized/) | Indicates whether to optimize the output elements. |
|[GetDefaultFont](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
|[SetDefaultFont](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
|[GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. |
|[SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. |
|[GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
|[SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
|[GetGridlineType](./getgridlinetype/) | Gets or sets gridline type. |
|[SetGridlineType](./setgridlinetype/) | Gets or sets gridline type. |
|[GetGridlineColor](./getgridlinecolor/) | Gets or sets gridline colr. |
|[SetGridlineColor](./setgridlinecolor/) | Gets or sets gridline colr. |
|[GetTextCrossType](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
|[SetTextCrossType](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
|[GetDefaultEditLanguage](./getdefaulteditlanguage/) | Gets or sets default edit language. |
|[SetDefaultEditLanguage](./setdefaulteditlanguage/) | Gets or sets default edit language. |
|[GetSheetSet](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[SetSheetSet](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[GetEmfRenderSetting](./getemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
|[SetEmfRenderSetting](./setemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
|[GetCustomRenderSettings](./getcustomrendersettings/) | Gets or sets custom settings during rendering. |
|[SetCustomRenderSettings](./setcustomrendersettings/) | Gets or sets custom settings during rendering. |
|[GetImageType](./getimagetype/) | Gets or sets the format of the generated images.default value: PNG. |
|[SetImageType](./setimagetype/) | Gets or sets the format of the generated images.default value: PNG. |
