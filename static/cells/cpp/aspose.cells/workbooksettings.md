##Aspose::Cells::WorkbookSettings class
'Aspose::Cells::WorkbookSettings class. Represents all settings of the workbook in C++.'
## WorkbookSettings class
Represents all settings of the workbook.
```cpp
class WorkbookSettings
```
## Methods
| Method | Description |
| --- | --- |
| [Dispose()](./dispose/) | Releases resources. |
| [GetAuthor()](./getauthor/) | Gets and sets the author of the file. |
| [GetAutoCompressPictures()](./getautocompresspictures/) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [GetAutoRecover()](./getautorecover/) | Indicates whether the file is marked for auto-recovery. |
| [GetBuildVersion()](./getbuildversion/) | Specifies the incremental public release of the application. |
| [GetCheckCompatibility()](./getcheckcompatibility/) | Indicates whether check compatibility with earlier versions when saving workbook. |
| [GetCheckCustomNumberFormat()](./getcheckcustomnumberformat/) | Indicates whether checking custom number format when setting Style.Custom. |
| [GetCheckExcelRestriction()](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetCompliance()](./getcompliance/) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [GetCrashSave()](./getcrashsave/) | indicates whether the application last saved the workbook file after a crash. |
| [GetDataExtractLoad()](./getdataextractload/) | indicates whether the application last opened the workbook for data recovery. |
| [GetDate1904()](./getdate1904/) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [GetDefaultImageResolution()](./getdefaultimageresolution/) | Gets and sets default resolution of image. |
| [GetDefaultStyleSettings()](./getdefaultstylesettings/) | Gets the settings for default values of style-related properties for this workbook. |
| [GetDiscardImageEditData()](./getdiscardimageeditdata/) | Indicates whether discarding editting image data. |
| [GetDisplayDrawingObjects()](./getdisplaydrawingobjects/) | Indicates whether and how to show objects in the workbook. |
| [GetEnableMacros()](./getenablemacros/) | Enable macros;. |
| [GetFirstVisibleTab()](./getfirstvisibletab/) | Gets or sets the first visible worksheet tab. |
| [GetFormulaSettings()](./getformulasettings/) | Gets the settings for formula-related features. |
| [GetGlobalizationSettings()](./getglobalizationsettings/) | Gets and sets the globalization settings. |
| [GetHidePivotFieldList()](./gethidepivotfieldlist/) | Gets and sets whether hide the field list for the PivotTable. |
| [GetLanguageCode()](./getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [GetMaxColumn()](./getmaxcolumn/) | Gets the max column index, zero-based. |
| [GetMaxRow()](./getmaxrow/) | Gets the max row index, zero-based. |
| [GetMaxRowsOfSharedFormula()](./getmaxrowsofsharedformula/) | Gets and sets the max row number of shared formula. |
| [GetMaxUniqueItemsPerField()](./getmaxuniqueitemsperfield/) | Gets and set the limitation of unique items per field. |
| [GetMemorySetting()](./getmemorysetting/) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [GetNumberDecimalSeparator()](./getnumberdecimalseparator/) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [GetNumberGroupSeparator()](./getnumbergroupseparator/) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [GetPaperSize()](./getpapersize/) | Gets and sets the default print paper size. |
| [GetPassword()](./getpassword/) | Represents [Workbook](../workbook/) file encryption password. |
| [GetPropertiesFollowChartPoint()](./getpropertiesfollowchartpoint/) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [GetProtectionType()](./getprotectiontype/) | Gets the protection type of the workbook. |
| [GetQuotePrefixToStyle()](./getquoteprefixtostyle/) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts  with single quote mark ) to the cell. |
| [GetRegion()](./getregion/) | Gets or sets the regional settings for workbook. |
| [GetRemovePersonalInformation()](./getremovepersonalinformation/) | True if personal information can be removed from the specified workbook. |
| [GetRepairLoad()](./getrepairload/) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [GetShared()](./getshared/) | Gets or sets a value that indicates whether the [Workbook](../workbook/) is shared. |
| [GetSheetTabBarWidth()](./getsheettabbarwidth/) | Width of worksheet tab bar (in 1/1000 of window width). |
| [GetShowTabs()](./getshowtabs/) | Get or sets a value whether the [Workbook](../workbook/) tabs are displayed. |
| [GetSignificantDigitsType()](./getsignificantdigitstype/) | Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is CellsHelper.SignificantDigitsType. |
| [GetSmartTagOptions()](./getsmarttagoptions/) | Gets the options of the smart tag. |
| [GetThemeFont(FontSchemeType type)](./getthemefont/) | Gets the default theme font name. |
| [GetUpdateAdjacentCellsBorder()](./getupdateadjacentcellsborder/) | Indicates whether update adjacent cells' border. |
| [GetUpdateLinksType()](./getupdatelinkstype/) | Gets and sets how updates external links when the workbook is opened. |
| [GetWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [GetWindowHeight()](./getwindowheight/) | The height of the window, in unit of point. |
| [GetWindowHeightCM()](./getwindowheightcm/) | The height of the window, in unit of centimeter. |
| [GetWindowHeightInch()](./getwindowheightinch/) | The height of the window, in unit of inch. |
| [GetWindowLeft()](./getwindowleft/) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [GetWindowLeftCM()](./getwindowleftcm/) | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [GetWindowLeftInch()](./getwindowleftinch/) | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [GetWindowTop()](./getwindowtop/) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [GetWindowTopCM()](./getwindowtopcm/) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [GetWindowTopInch()](./getwindowtopinch/) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [GetWindowWidth()](./getwindowwidth/) | The width of the window, in unit of point. |
| [GetWindowWidthCM()](./getwindowwidthcm/) | The width of the window, in unit of centimeter. |
| [GetWindowWidthInch()](./getwindowwidthinch/) | The width of the window, in unit of inch. |
| [GetWriteProtection()](./getwriteprotection/) | Provides access to the workbook write protection options. |
| [IsDefaultEncrypted()](./isdefaultencrypted/) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [IsEncrypted()](./isencrypted/) | Gets a value that indicates whether a password is required to open this workbook. |
| [IsHidden()](./ishidden/) | Indicates whether this workbook is hidden. |
| [IsHScrollBarVisible()](./ishscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [IsMinimized()](./isminimized/) | Represents whether the generated spreadsheet will be opened Minimized. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsProtected()](./isprotected/) | Gets a value that indicates whether the structure or window of the [Workbook](../workbook/) is protected. |
| [IsVScrollBarVisible()](./isvscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WorkbookSettings\& src)](./operator_asm/) | operator= |
| [SetAuthor(const U16String\& value)](./setauthor/) | Gets and sets the author of the file. |
| [SetAuthor(const char16_t* value)](./setauthor/) | Gets and sets the author of the file. |
| [SetAutoCompressPictures(bool value)](./setautocompresspictures/) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [SetAutoRecover(bool value)](./setautorecover/) | Indicates whether the file is marked for auto-recovery. |
| [SetBuildVersion(const U16String\& value)](./setbuildversion/) | Specifies the incremental public release of the application. |
| [SetBuildVersion(const char16_t* value)](./setbuildversion/) | Specifies the incremental public release of the application. |
| [SetCheckCompatibility(bool value)](./setcheckcompatibility/) | Indicates whether check compatibility with earlier versions when saving workbook. |
| [SetCheckCustomNumberFormat(bool value)](./setcheckcustomnumberformat/) | Indicates whether checking custom number format when setting Style.Custom. |
| [SetCheckExcelRestriction(bool value)](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetCompliance(OoxmlCompliance value)](./setcompliance/) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [SetCrashSave(bool value)](./setcrashsave/) | indicates whether the application last saved the workbook file after a crash. |
| [SetDataExtractLoad(bool value)](./setdataextractload/) | indicates whether the application last opened the workbook for data recovery. |
| [SetDate1904(bool value)](./setdate1904/) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [SetDefaultImageResolution(int32_t value)](./setdefaultimageresolution/) | Gets and sets default resolution of image. |
| [SetDiscardImageEditData(bool value)](./setdiscardimageeditdata/) | Indicates whether discarding editting image data. |
| [SetDisplayDrawingObjects(DisplayDrawingObjects value)](./setdisplaydrawingobjects/) | Indicates whether and how to show objects in the workbook. |
| [SetEnableMacros(bool value)](./setenablemacros/) | Enable macros;. |
| [SetFirstVisibleTab(int32_t value)](./setfirstvisibletab/) | Gets or sets the first visible worksheet tab. |
| [SetGlobalizationSettings(GlobalizationSettings* value)](./setglobalizationsettings/) | Gets and sets the globalization settings. |
| [SetHidePivotFieldList(bool value)](./sethidepivotfieldlist/) | Gets and sets whether hide the field list for the PivotTable. |
| [SetIsDefaultEncrypted(bool value)](./setisdefaultencrypted/) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [SetIsHidden(bool value)](./setishidden/) | Indicates whether this workbook is hidden. |
| [SetIsHScrollBarVisible(bool value)](./setishscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [SetIsMinimized(bool value)](./setisminimized/) | Represents whether the generated spreadsheet will be opened Minimized. |
| [SetIsVScrollBarVisible(bool value)](./setisvscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [SetLanguageCode(CountryCode value)](./setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetMaxRowsOfSharedFormula(int32_t value)](./setmaxrowsofsharedformula/) | Gets and sets the max row number of shared formula. |
| [SetMaxUniqueItemsPerField(int32_t value)](./setmaxuniqueitemsperfield/) | Gets and set the limitation of unique items per field. |
| [SetMemorySetting(MemorySetting value)](./setmemorysetting/) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [SetNumberDecimalSeparator(char16_t value)](./setnumberdecimalseparator/) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [SetNumberGroupSeparator(char16_t value)](./setnumbergroupseparator/) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [SetPageOrientationType(PageOrientationType pageOrientationType)](./setpageorientationtype/) | Set the type of print orientation for the whole workbook. |
| [SetPaperSize(PaperSizeType value)](./setpapersize/) | Gets and sets the default print paper size. |
| [SetPassword(const U16String\& value)](./setpassword/) | Represents [Workbook](../workbook/) file encryption password. |
| [SetPassword(const char16_t* value)](./setpassword/) | Represents [Workbook](../workbook/) file encryption password. |
| [SetPropertiesFollowChartPoint(bool value)](./setpropertiesfollowchartpoint/) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [SetQuotePrefixToStyle(bool value)](./setquoteprefixtostyle/) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts  with single quote mark ) to the cell. |
| [SetRegion(CountryCode value)](./setregion/) | Gets or sets the regional settings for workbook. |
| [SetRemovePersonalInformation(bool value)](./setremovepersonalinformation/) | True if personal information can be removed from the specified workbook. |
| [SetRepairLoad(bool value)](./setrepairload/) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [SetShared(bool value)](./setshared/) | Gets or sets a value that indicates whether the [Workbook](../workbook/) is shared. |
| [SetSheetTabBarWidth(int32_t value)](./setsheettabbarwidth/) | Width of worksheet tab bar (in 1/1000 of window width). |
| [SetShowTabs(bool value)](./setshowtabs/) | Get or sets a value whether the [Workbook](../workbook/) tabs are displayed. |
| [SetSignificantDigitsType(SignificantDigitsType value)](./setsignificantdigitstype/) | Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is CellsHelper.SignificantDigitsType. |
| [SetUpdateAdjacentCellsBorder(bool value)](./setupdateadjacentcellsborder/) | Indicates whether update adjacent cells' border. |
| [SetUpdateLinksType(UpdateLinksType value)](./setupdatelinkstype/) | Gets and sets how updates external links when the workbook is opened. |
| [SetWarningCallback(IWarningCallback* value)](./setwarningcallback/) | Gets or sets warning callback. |
| [SetWindowHeight(double value)](./setwindowheight/) | The height of the window, in unit of point. |
| [SetWindowHeightCM(double value)](./setwindowheightcm/) | The height of the window, in unit of centimeter. |
| [SetWindowHeightInch(double value)](./setwindowheightinch/) | The height of the window, in unit of inch. |
| [SetWindowLeft(double value)](./setwindowleft/) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [SetWindowLeftCM(double value)](./setwindowleftcm/) | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [SetWindowLeftInch(double value)](./setwindowleftinch/) | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [SetWindowTop(double value)](./setwindowtop/) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [SetWindowTopCM(double value)](./setwindowtopcm/) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [SetWindowTopInch(double value)](./setwindowtopinch/) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [SetWindowWidth(double value)](./setwindowwidth/) | The width of the window, in unit of point. |
| [SetWindowWidthCM(double value)](./setwindowwidthcm/) | The width of the window, in unit of centimeter. |
| [SetWindowWidthInch(double value)](./setwindowwidthinch/) | The width of the window, in unit of inch. |
| [WorkbookSettings(WorkbookSettings_Impl* impl)](./workbooksettings/) | Constructs from an implementation object. |
| [WorkbookSettings(const WorkbookSettings\& src)](./workbooksettings/) | Copy constructor. |
| [~WorkbookSettings()](./~workbooksettings/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
WorkbookSettings settings = workbook.GetSettings();
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
