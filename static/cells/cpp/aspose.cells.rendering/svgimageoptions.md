##Aspose::Cells::Rendering::SvgImageOptions class
'Aspose::Cells::Rendering::SvgImageOptions class. Options for generating Svg image in C++.'
## SvgImageOptions class
Options for generating Svg image.
```cpp
class SvgImageOptions : public Aspose::Cells::Rendering::ImageOrPrintOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAllColumnsInOnePagePerSheet()](../imageorprintoptions/getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [GetCheckWorkbookDefaultFont()](../imageorprintoptions/getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [GetCssPrefix()](./getcssprefix/) | Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [GetCustomRenderSettings()](../imageorprintoptions/getcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [GetDefaultEditLanguage()](../imageorprintoptions/getdefaulteditlanguage/) | Gets or sets default edit language. |
| [GetDefaultFont()](../imageorprintoptions/getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [GetDrawObjectEventHandler()](../imageorprintoptions/getdrawobjecteventhandler/) | Implements this interface to get [DrawObject](../drawobject/) and Bound when rendering. |
| [GetEmbeddedFontType()](./getembeddedfonttype/) | Gets or sets the type of font that embedded in Svg. |
| [GetEmbededImageNameInSvg()](../imageorprintoptions/getembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [GetEmfRenderSetting()](../imageorprintoptions/getemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
| [GetFitToViewPort()](./getfittoviewport/) | if this property is true, the generated svg will fit to view port. |
| [GetGridlineColor()](../imageorprintoptions/getgridlinecolor/) | Gets or sets gridline colr. |
| [GetGridlineType()](../imageorprintoptions/getgridlinetype/) | Gets or sets gridline type. |
| [GetHorizontalResolution()](../imageorprintoptions/gethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [GetImageType()](./getimagetype/) | Gets or sets the format of the generated images. default value: PNG. |
| [GetOnePagePerSheet()](../imageorprintoptions/getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [GetOnlyArea()](../imageorprintoptions/getonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
| [GetOutputBlankPageWhenNothingToPrint()](../imageorprintoptions/getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [GetPageCount()](../imageorprintoptions/getpagecount/) | Gets or sets the number of pages to save. |
| [GetPageIndex()](../imageorprintoptions/getpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [GetPageSavingCallback()](../imageorprintoptions/getpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [GetPrintingPage()](../imageorprintoptions/getprintingpage/) | Indicates which pages will not be printed. |
| [GetPrintWithStatusDialog()](../imageorprintoptions/getprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [GetQuality()](../imageorprintoptions/getquality/) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the **Jpeg** format. The default value is 100. |
| [GetSheetSet()](../imageorprintoptions/getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetSvgCssPrefix()](../imageorprintoptions/getsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [GetSVGFitToViewPort()](../imageorprintoptions/getsvgfittoviewport/) |  **(Deprecated)** if this property is true, the generated svg will fit to view port. |
| [GetTextCrossType()](../imageorprintoptions/gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [GetTiffBinarizationMethod()](../imageorprintoptions/gettiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp format when [ImageType](../../aspose.cells.drawing/imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [GetTiffColorDepth()](../imageorprintoptions/gettiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the **Tiff** format. |
| [GetTiffCompression()](../imageorprintoptions/gettiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the **Tiff** format. |
| [GetTransparent()](../imageorprintoptions/gettransparent/) | Indicates if the background of generated image should be transparent. |
| [GetVerticalResolution()](../imageorprintoptions/getverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [GetWarningCallback()](../imageorprintoptions/getwarningcallback/) | Gets or sets warning callback. |
| [ImageOrPrintOptions()](../imageorprintoptions/imageorprintoptions/) | Ctor. |
| [ImageOrPrintOptions(ImageOrPrintOptions_Impl* impl)](../imageorprintoptions/imageorprintoptions/) | Constructs from an implementation object. |
| [ImageOrPrintOptions(const ImageOrPrintOptions\& src)](../imageorprintoptions/imageorprintoptions/) | Copy constructor. |
| [IsFontSubstitutionCharGranularity()](../imageorprintoptions/isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOptimized()](../imageorprintoptions/isoptimized/) | Indicates whether to optimize the output elements. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SvgImageOptions\& src)](./operator_asm/) | operator= |
| [operator=(const ImageOrPrintOptions\& src)](../imageorprintoptions/operator_asm/) | operator= |
| [SetAllColumnsInOnePagePerSheet(bool value)](../imageorprintoptions/setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [SetCheckWorkbookDefaultFont(bool value)](../imageorprintoptions/setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [SetCssPrefix(const U16String\& value)](./setcssprefix/) | Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetCssPrefix(const char16_t* value)](./setcssprefix/) | Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetCustomRenderSettings(const CustomRenderSettings\& value)](../imageorprintoptions/setcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [SetDefaultEditLanguage(DefaultEditLanguage value)](../imageorprintoptions/setdefaulteditlanguage/) | Gets or sets default edit language. |
| [SetDefaultFont(const U16String\& value)](../imageorprintoptions/setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [SetDefaultFont(const char16_t* value)](../imageorprintoptions/setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../../aspose.cells/) will use system default font to show these unicode characters. |
| [SetDesiredSize(int32_t desiredWidth, int32_t desiredHeight, bool keepAspectRatio)](../imageorprintoptions/setdesiredsize/) | Sets desired width and height of image. |
| [SetDrawObjectEventHandler(DrawObjectEventHandler* value)](../imageorprintoptions/setdrawobjecteventhandler/) | Implements this interface to get [DrawObject](../drawobject/) and Bound when rendering. |
| [SetEmbeddedFontType(SvgEmbeddedFontType value)](./setembeddedfonttype/) | Gets or sets the type of font that embedded in Svg. |
| [SetEmbededImageNameInSvg(const U16String\& value)](../imageorprintoptions/setembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [SetEmbededImageNameInSvg(const char16_t* value)](../imageorprintoptions/setembededimagenameinsvg/) |  **(Deprecated)** Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded". |
| [SetEmfRenderSetting(EmfRenderSetting value)](../imageorprintoptions/setemfrendersetting/) | Setting for rendering Emf metafiles in source file. |
| [SetFitToViewPort(bool value)](./setfittoviewport/) | if this property is true, the generated svg will fit to view port. |
| [SetGridlineColor(const Aspose::Cells::Color\& value)](../imageorprintoptions/setgridlinecolor/) | Gets or sets gridline colr. |
| [SetGridlineType(GridlineType value)](../imageorprintoptions/setgridlinetype/) | Gets or sets gridline type. |
| [SetHorizontalResolution(int32_t value)](../imageorprintoptions/sethorizontalresolution/) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [SetImageType(Aspose::Cells::Drawing::ImageType value)](./setimagetype/) | Gets or sets the format of the generated images. default value: PNG. |
| [SetIsFontSubstitutionCharGranularity(bool value)](../imageorprintoptions/setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [SetIsOptimized(bool value)](../imageorprintoptions/setisoptimized/) | Indicates whether to optimize the output elements. |
| [SetOnePagePerSheet(bool value)](../imageorprintoptions/setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [SetOnlyArea(bool value)](../imageorprintoptions/setonlyarea/) | If this property is true , one Area will be output, and no scale will take effect. |
| [SetOutputBlankPageWhenNothingToPrint(bool value)](../imageorprintoptions/setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [SetPageCount(int32_t value)](../imageorprintoptions/setpagecount/) | Gets or sets the number of pages to save. |
| [SetPageIndex(int32_t value)](../imageorprintoptions/setpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [SetPageSavingCallback(IPageSavingCallback* value)](../imageorprintoptions/setpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [SetPrintingPage(PrintingPageType value)](../imageorprintoptions/setprintingpage/) | Indicates which pages will not be printed. |
| [SetPrintWithStatusDialog(bool value)](../imageorprintoptions/setprintwithstatusdialog/) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [SetQuality(int32_t value)](../imageorprintoptions/setquality/) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the **Jpeg** format. The default value is 100. |
| [SetSheetSet(const SheetSet\& value)](../imageorprintoptions/setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSvgCssPrefix(const U16String\& value)](../imageorprintoptions/setsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetSvgCssPrefix(const char16_t* value)](../imageorprintoptions/setsvgcssprefix/) |  **(Deprecated)** Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SetSVGFitToViewPort(bool value)](../imageorprintoptions/setsvgfittoviewport/) |  **(Deprecated)** if this property is true, the generated svg will fit to view port. |
| [SetTextCrossType(TextCrossType value)](../imageorprintoptions/settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [SetTiffBinarizationMethod(ImageBinarizationMethod value)](../imageorprintoptions/settiffbinarizationmethod/) | Gets or sets method used while converting images to 1 bpp format when [ImageType](../../aspose.cells.drawing/imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [SetTiffColorDepth(ColorDepth value)](../imageorprintoptions/settiffcolordepth/) | Gets or sets bit depth to apply only when saving pages to the **Tiff** format. |
| [SetTiffCompression(TiffCompression value)](../imageorprintoptions/settiffcompression/) | Gets or sets the type of compression to apply only when saving pages to the **Tiff** format. |
| [SetTransparent(bool value)](../imageorprintoptions/settransparent/) | Indicates if the background of generated image should be transparent. |
| [SetVerticalResolution(int32_t value)](../imageorprintoptions/setverticalresolution/) | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [SetWarningCallback(IWarningCallback* value)](../imageorprintoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SvgImageOptions()](./svgimageoptions/) | Ctor. |
| [SvgImageOptions(SvgImageOptions_Impl* impl)](./svgimageoptions/) | Constructs from an implementation object. |
| [SvgImageOptions(const SvgImageOptions\& src)](./svgimageoptions/) | Copy constructor. |
| [SvgImageOptions(const ImageOrPrintOptions\& src)](./svgimageoptions/) | Constructs from a parent object. |
| [~ImageOrPrintOptions()](../imageorprintoptions/~imageorprintoptions/) | Destructor. |
| [~SvgImageOptions()](./~svgimageoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [ImageOrPrintOptions](../imageorprintoptions/)
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
