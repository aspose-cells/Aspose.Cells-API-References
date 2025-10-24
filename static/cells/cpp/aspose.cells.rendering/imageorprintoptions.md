##Aspose::Cells::Rendering::ImageOrPrintOptions class
'Aspose::Cells::Rendering::ImageOrPrintOptions class. Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image in C++.'
## ImageOrPrintOptions class
Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.
```cpp
class ImageOrPrintOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAllColumnsInOnePagePerSheet()](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [GetCheckWorkbookDefaultFont()](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [GetCustomRenderSettings()](./getcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [GetDefaultEditLanguage()](./getdefaulteditlanguage/) | Gets or sets default edit language. |
| [GetDefaultFont()](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [GetDrawObjectEventHandler()](./getdrawobjecteventhandler/) | Implements this interface to get [DrawObject](../drawobject/) and Bound when rendering. |
| [GetEmbededImageNameInSvg()](./getembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [GetEmfRenderSetting()](./getemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
| [GetGridlineColor()](./getgridlinecolor/) | Gets or sets gridline colr. |
| [GetGridlineType()](./getgridlinetype/) | Gets or sets gridline type. |
| [GetHorizontalResolution()](./gethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [GetImageType()](./getimagetype/) | Gets or sets the format of the generated images. default value: PNG. |
| [GetOnePagePerSheet()](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [GetOnlyArea()](./getonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
| [GetOutputBlankPageWhenNothingToPrint()](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [GetPageCount()](./getpagecount/) | Gets or sets the number of pages to save. |
| [GetPageIndex()](./getpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [GetPageSavingCallback()](./getpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [GetPrintingPage()](./getprintingpage/) | Indicates which pages will not be printed. |
| [GetPrintWithStatusDialog()](./getprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [GetQuality()](./getquality/) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the **Jpeg** format. The default value is 100. |
| [GetSheetSet()](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetSvgCssPrefix()](./getsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [GetSVGFitToViewPort()](./getsvgfittoviewport/) |  **(Deprecated)** if this property is true, the generated svg will fit to view port. |
| [GetTextCrossType()](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [GetTiffBinarizationMethod()](./gettiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp format when [ImageType](../../aspose.cells.drawing/imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [GetTiffColorDepth()](./gettiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the **Tiff** format. |
| [GetTiffCompression()](./gettiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the **Tiff** format. |
| [GetTransparent()](./gettransparent/) | Indicates if the background of generated image should be transparent. |
| [GetVerticalResolution()](./getverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [GetWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [ImageOrPrintOptions()](./imageorprintoptions/) | Ctor. |
| [ImageOrPrintOptions(ImageOrPrintOptions_Impl* impl)](./imageorprintoptions/) | Constructs from an implementation object. |
| [ImageOrPrintOptions(const ImageOrPrintOptions\& src)](./imageorprintoptions/) | Copy constructor. |
| [IsFontSubstitutionCharGranularity()](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOptimized()](./isoptimized/) | Indicates whether to optimize the output elements. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ImageOrPrintOptions\& src)](./operator_asm/) | operator= |
| [SetAllColumnsInOnePagePerSheet(bool value)](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [SetCheckWorkbookDefaultFont(bool value)](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [SetCustomRenderSettings(const CustomRenderSettings\& value)](./setcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [SetDefaultEditLanguage(DefaultEditLanguage value)](./setdefaulteditlanguage/) | Gets or sets default edit language. |
| [SetDefaultFont(const U16String\& value)](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [SetDefaultFont(const char16_t* value)](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [SetDesiredSize(int32_t desiredWidth, int32_t desiredHeight, bool keepAspectRatio)](./setdesiredsize/) | Sets desired width and height of image. |
| [SetDrawObjectEventHandler(DrawObjectEventHandler* value)](./setdrawobjecteventhandler/) | Implements this interface to get [DrawObject](../drawobject/) and Bound when rendering. |
| [SetEmbededImageNameInSvg(const U16String\& value)](./setembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [SetEmbededImageNameInSvg(const char16_t* value)](./setembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [SetEmfRenderSetting(EmfRenderSetting value)](./setemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
| [SetGridlineColor(const Aspose::Cells::Color\& value)](./setgridlinecolor/) | Gets or sets gridline colr. |
| [SetGridlineType(GridlineType value)](./setgridlinetype/) | Gets or sets gridline type. |
| [SetHorizontalResolution(int32_t value)](./sethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [SetImageType(Aspose::Cells::Drawing::ImageType value)](./setimagetype/) | Gets or sets the format of the generated images. default value: PNG. |
| [SetIsFontSubstitutionCharGranularity(bool value)](./setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [SetIsOptimized(bool value)](./setisoptimized/) | Indicates whether to optimize the output elements. |
| [SetOnePagePerSheet(bool value)](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [SetOnlyArea(bool value)](./setonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
| [SetOutputBlankPageWhenNothingToPrint(bool value)](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [SetPageCount(int32_t value)](./setpagecount/) | Gets or sets the number of pages to save. |
| [SetPageIndex(int32_t value)](./setpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [SetPageSavingCallback(IPageSavingCallback* value)](./setpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [SetPrintingPage(PrintingPageType value)](./setprintingpage/) | Indicates which pages will not be printed. |
| [SetPrintWithStatusDialog(bool value)](./setprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [SetQuality(int32_t value)](./setquality/) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the **Jpeg** format. The default value is 100. |
| [SetSheetSet(const SheetSet\& value)](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSvgCssPrefix(const U16String\& value)](./setsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetSvgCssPrefix(const char16_t* value)](./setsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetSVGFitToViewPort(bool value)](./setsvgfittoviewport/) |  **(Deprecated)** if this property is true, the generated svg will fit to view port. |
| [SetTextCrossType(TextCrossType value)](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [SetTiffBinarizationMethod(ImageBinarizationMethod value)](./settiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp format when [ImageType](../../aspose.cells.drawing/imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [SetTiffColorDepth(ColorDepth value)](./settiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the **Tiff** format. |
| [SetTiffCompression(TiffCompression value)](./settiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the **Tiff** format. |
| [SetTransparent(bool value)](./settransparent/) | Indicates if the background of generated image should be transparent. |
| [SetVerticalResolution(int32_t value)](./setverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [SetWarningCallback(IWarningCallback* value)](./setwarningcallback/) | Gets or sets warning callback. |
| [~ImageOrPrintOptions()](./~imageorprintoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Set Image Or Print Options
ImageOrPrintOptions options;
//Set output image format
options.SetImageType(ImageType::Png);
//Set Horizontal resolution
options.SetHorizontalResolution(300);
//Set Vertical Resolution
options.SetVerticalResolution(300);
//Instantiate Workbook
Workbook book(u"test.xls");
//Save chart as Image using ImageOrPrint Options
book.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"chart.png", options);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
