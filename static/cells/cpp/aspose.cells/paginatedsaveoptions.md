##Aspose::Cells::PaginatedSaveOptions class
'Aspose::Cells::PaginatedSaveOptions class. Represents the options for pagination in C++.'
## PaginatedSaveOptions class
Represents the options for pagination.
```cpp
class PaginatedSaveOptions : public Aspose::Cells::SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAllColumnsInOnePagePerSheet()](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetCheckFontCompatibility()](./getcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. |
| [GetCheckWorkbookDefaultFont()](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetCustomRenderSettings()](./getcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [GetDefaultEditLanguage()](./getdefaulteditlanguage/) | Gets or sets default edit language. |
| [GetDefaultFont()](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../) will use system default font to show these unicode characters. |
| [GetDrawObjectEventHandler()](./getdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
| [GetEmfRenderSetting()](./getemfrendersetting/) | Setting for rendering Emf metafile. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetGridlineColor()](./getgridlinecolor/) | Gets or sets gridline color. |
| [GetGridlineType()](./getgridlinetype/) | Gets or sets gridline type. |
| [GetIgnoreError()](./getignoreerror/) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetOnePagePerSheet()](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [GetOutputBlankPageWhenNothingToPrint()](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [GetPageCount()](./getpagecount/) | Gets or sets the number of pages to save. |
| [GetPageIndex()](./getpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [GetPageSavingCallback()](./getpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [GetPrintingPageType()](./getprintingpagetype/) | Indicates which pages will not be printed. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSheetSet()](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetTextCrossType()](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsFontSubstitutionCharGranularity()](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PaginatedSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [PaginatedSaveOptions(PaginatedSaveOptions_Impl* impl)](./paginatedsaveoptions/) | Constructs from an implementation object. |
| [PaginatedSaveOptions(const PaginatedSaveOptions\& src)](./paginatedsaveoptions/) | Copy constructor. |
| [PaginatedSaveOptions(const SaveOptions\& src)](./paginatedsaveoptions/) | Constructs from a parent object. |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetAllColumnsInOnePagePerSheet(bool value)](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetCheckFontCompatibility(bool value)](./setcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. |
| [SetCheckWorkbookDefaultFont(bool value)](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetCustomRenderSettings(const CustomRenderSettings\& value)](./setcustomrendersettings/) | Gets or sets custom settings during rendering. |
| [SetDefaultEditLanguage(DefaultEditLanguage value)](./setdefaulteditlanguage/) | Gets or sets default edit language. |
| [SetDefaultFont(const U16String\& value)](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../) will use system default font to show these unicode characters. |
| [SetDefaultFont(const char16_t* value)](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, [Aspose.Cells](../) will use system default font to show these unicode characters. |
| [SetDrawObjectEventHandler(DrawObjectEventHandler* value)](./setdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
| [SetEmfRenderSetting(EmfRenderSetting value)](./setemfrendersetting/) | Setting for rendering Emf metafile. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetGridlineColor(const Aspose::Cells::Color\& value)](./setgridlinecolor/) | Gets or sets gridline color. |
| [SetGridlineType(GridlineType value)](./setgridlinetype/) | Gets or sets gridline type. |
| [SetIgnoreError(bool value)](./setignoreerror/) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [SetIsFontSubstitutionCharGranularity(bool value)](./setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetOnePagePerSheet(bool value)](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [SetOutputBlankPageWhenNothingToPrint(bool value)](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
| [SetPageCount(int32_t value)](./setpagecount/) | Gets or sets the number of pages to save. |
| [SetPageIndex(int32_t value)](./setpageindex/) | Gets or sets the 0-based index of the first page to save. |
| [SetPageSavingCallback(IPageSavingCallback* value)](./setpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [SetPrintingPageType(PrintingPageType value)](./setprintingpagetype/) | Indicates which pages will not be printed. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSheetSet(const SheetSet\& value)](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetTextCrossType(TextCrossType value)](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~PaginatedSaveOptions()](./~paginatedsaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
