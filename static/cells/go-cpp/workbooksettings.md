##WorkbookSettings Class
'WorkbookSettings class. Encapsulates the object that represents workbooksettings in Go.'
## WorkbookSettings class
Represents all settings of the workbook.
```go
type WorkbookSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Dispose](./dispose/) | Releases resources. |
|[GetThemeFont](./getthemefont/) | Gets the default theme font name. |
|[GetAuthor](./getauthor/) | Gets and sets the author of the file. |
|[SetAuthor](./setauthor/) | Gets and sets the author of the file. |
|[GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Indicates whether checking custom number format when setting Style.Custom. |
|[SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Indicates whether checking custom number format when setting Style.Custom. |
|[GetEnableMacros](./getenablemacros/) | Enable macros; |
|[SetEnableMacros](./setenablemacros/) | Enable macros; |
|[GetDate1904](./getdate1904/) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
|[SetDate1904](./setdate1904/) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
|[GetProtectionType](./getprotectiontype/) | Gets the protection type of the workbook. |
|[GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Indicates whether and how to show objects in the workbook. |
|[SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Indicates whether and how to show objects in the workbook. |
|[GetSheetTabBarWidth](./getsheettabbarwidth/) | Width of worksheet tab bar (in 1/1000 of window width). |
|[SetSheetTabBarWidth](./setsheettabbarwidth/) | Width of worksheet tab bar (in 1/1000 of window width). |
|[GetShowTabs](./getshowtabs/) | Get or sets a value whether the Workbook tabs are displayed. |
|[SetShowTabs](./setshowtabs/) | Get or sets a value whether the Workbook tabs are displayed. |
|[GetFirstVisibleTab](./getfirstvisibletab/) | Gets or sets the first visible worksheet tab. |
|[SetFirstVisibleTab](./setfirstvisibletab/) | Gets or sets the first visible worksheet tab. |
|[IsHScrollBarVisible](./ishscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
|[SetIsHScrollBarVisible](./setishscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
|[IsVScrollBarVisible](./isvscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
|[SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
|[GetShared](./getshared/) | Gets or sets a value that indicates whether the Workbook is shared. |
|[SetShared](./setshared/) | Gets or sets a value that indicates whether the Workbook is shared. |
|[GetLanguageCode](./getlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
|[SetLanguageCode](./setlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
|[GetRegion](./getregion/) | Gets or sets the regional settings for workbook. |
|[SetRegion](./setregion/) | Gets or sets the regional settings for workbook. |
|[GetGlobalizationSettings](./getglobalizationsettings/) | Gets and sets the globalization settings. |
|[SetGlobalizationSettings](./setglobalizationsettings/) | Gets and sets the globalization settings. |
|[GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
|[SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
|[GetNumberGroupSeparator](./getnumbergroupseparator/) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
|[SetNumberGroupSeparator](./setnumbergroupseparator/) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
|[GetPassword](./getpassword/) | Represents Workbook file encryption password. |
|[SetPassword](./setpassword/) | Represents Workbook file encryption password. |
|[GetWriteProtection](./getwriteprotection/) | Provides access to the workbook write protection options. |
|[IsEncrypted](./isencrypted/) | Gets a value that indicates whether a password is required to open this workbook. |
|[IsProtected](./isprotected/) | Gets a value that indicates whether the structure or window of the Workbook is protected. |
|[IsDefaultEncrypted](./isdefaultencrypted/) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
|[SetIsDefaultEncrypted](./setisdefaultencrypted/) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
|[IsMinimized](./isminimized/) | Represents whether the generated spreadsheet will be opened Minimized. |
|[SetIsMinimized](./setisminimized/) | Represents whether the generated spreadsheet will be opened Minimized. |
|[IsHidden](./ishidden/) | Indicates whether this workbook is hidden. |
|[SetIsHidden](./setishidden/) | Indicates whether this workbook is hidden. |
|[GetAutoCompressPictures](./getautocompresspictures/) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
|[SetAutoCompressPictures](./setautocompresspictures/) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
|[GetRemovePersonalInformation](./getremovepersonalinformation/) | True if personal information can be removed from the specified workbook. |
|[SetRemovePersonalInformation](./setremovepersonalinformation/) | True if personal information can be removed from the specified workbook. |
|[GetHidePivotFieldList](./gethidepivotfieldlist/) | Gets and sets whether hide the field list for the PivotTable. |
|[SetHidePivotFieldList](./sethidepivotfieldlist/) | Gets and sets whether hide the field list for the PivotTable. |
|[GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Gets and set the limitation of unique items per field |
|[SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Gets and set the limitation of unique items per field |
|[GetUpdateLinksType](./getupdatelinkstype/) | Gets and sets how updates external links when the workbook is opened. |
|[SetUpdateLinksType](./setupdatelinkstype/) | Gets and sets how updates external links when the workbook is opened. |
|[SetPageOrientationType](./setpageorientationtype/) | Set the type of  print orientation for the whole workbook. |
|[GetMaxRow](./getmaxrow/) | Gets the max row index, zero-based. |
|[GetMaxColumn](./getmaxcolumn/) | Gets the max column index, zero-based. |
|[GetSmartTagOptions](./getsmarttagoptions/) | Gets the options of the smart tag. |
|[GetDefaultStyleSettings](./getdefaultstylesettings/) | Gets the settings for default values of style-related properties for this workbook. |
|[GetWindowLeft](./getwindowleft/) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
|[SetWindowLeft](./setwindowleft/) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
|[GetWindowLeftInch](./getwindowleftinch/) | The distance from the left edge of the client area to the left edge of the window.In unit of inch. |
|[SetWindowLeftInch](./setwindowleftinch/) | The distance from the left edge of the client area to the left edge of the window.In unit of inch. |
|[GetWindowLeftCM](./getwindowleftcm/) | The distance from the left edge of the client area to the left edge of the window.In unit of centimeter. |
|[SetWindowLeftCM](./setwindowleftcm/) | The distance from the left edge of the client area to the left edge of the window.In unit of centimeter. |
|[GetWindowTop](./getwindowtop/) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
|[SetWindowTop](./setwindowtop/) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
|[GetWindowTopInch](./getwindowtopinch/) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
|[SetWindowTopInch](./setwindowtopinch/) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
|[GetWindowTopCM](./getwindowtopcm/) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
|[SetWindowTopCM](./setwindowtopcm/) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
|[GetWindowWidth](./getwindowwidth/) | The width of the window, in unit of point. |
|[SetWindowWidth](./setwindowwidth/) | The width of the window, in unit of point. |
|[GetWindowWidthInch](./getwindowwidthinch/) | The width of the window, in unit of inch. |
|[SetWindowWidthInch](./setwindowwidthinch/) | The width of the window, in unit of inch. |
|[GetWindowWidthCM](./getwindowwidthcm/) | The width of the window, in unit of centimeter. |
|[SetWindowWidthCM](./setwindowwidthcm/) | The width of the window, in unit of centimeter. |
|[GetWindowHeight](./getwindowheight/) | The height of the window, in unit of point. |
|[SetWindowHeight](./setwindowheight/) | The height of the window, in unit of point. |
|[GetWindowHeightInch](./getwindowheightinch/) | The height of the window, in unit of inch. |
|[SetWindowHeightInch](./setwindowheightinch/) | The height of the window, in unit of inch. |
|[GetWindowHeightCM](./getwindowheightcm/) | The height of the window, in unit of centimeter. |
|[SetWindowHeightCM](./setwindowheightcm/) | The height of the window, in unit of centimeter. |
|[GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Indicates whether update adjacent cells' border. |
|[SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Indicates whether update adjacent cells' border. |
|[GetSignificantDigitsType](./getsignificantdigitstype/) | Gets and sets the type of significant digits for outputing numericvalues in this workbook. Default value is CellsHelper.SignificantDigitsType. |
|[SetSignificantDigitsType](./setsignificantdigitstype/) | Gets and sets the type of significant digits for outputing numericvalues in this workbook. Default value is CellsHelper.SignificantDigitsType. |
|[GetCheckCompatibility](./getcheckcompatibility/) | Indicates whether check compatibility with earlier versions when saving workbook. |
|[SetCheckCompatibility](./setcheckcompatibility/) | Indicates whether check compatibility with earlier versions when saving workbook. |
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
|[GetAutoRecover](./getautorecover/) | Indicates whether the file is marked for auto-recovery. |
|[SetAutoRecover](./setautorecover/) | Indicates whether the file is marked for auto-recovery. |
|[GetCrashSave](./getcrashsave/) | indicates whether the application last saved the workbook file after a crash. |
|[SetCrashSave](./setcrashsave/) | indicates whether the application last saved the workbook file after a crash. |
|[GetDataExtractLoad](./getdataextractload/) | indicates whether the application last opened the workbook for data recovery. |
|[SetDataExtractLoad](./setdataextractload/) | indicates whether the application last opened the workbook for data recovery. |
|[GetRepairLoad](./getrepairload/) | Indicates whether the application last opened the workbook in safe or repair mode. |
|[SetRepairLoad](./setrepairload/) | Indicates whether the application last opened the workbook in safe or repair mode. |
|[GetBuildVersion](./getbuildversion/) | Specifies the incremental public release of the application. |
|[SetBuildVersion](./setbuildversion/) | Specifies the incremental public release of the application. |
|[GetMemorySetting](./getmemorysetting/) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
|[SetMemorySetting](./setmemorysetting/) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
|[GetPaperSize](./getpapersize/) | Gets and sets the default print paper size. |
|[SetPaperSize](./setpapersize/) | Gets and sets the default print paper size. |
|[GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Gets and sets the max row number of shared formula. |
|[SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Gets and sets the max row number of shared formula. |
|[GetCompliance](./getcompliance/) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
|[SetCompliance](./setcompliance/) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
|[GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts  with single quote mark ) to the cell |
|[SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts  with single quote mark ) to the cell |
|[GetFormulaSettings](./getformulasettings/) | Gets the settings for formula-related features. |
|[GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
|[SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
|[GetDiscardImageEditData](./getdiscardimageeditdata/) | Indicates whether discarding editting image data. |
|[SetDiscardImageEditData](./setdiscardimageeditdata/) | Indicates whether discarding editting image data. |
|[GetDefaultImageResolution](./getdefaultimageresolution/) | Gets and sets default resolution of image. |
|[SetDefaultImageResolution](./setdefaultimageresolution/) | Gets and sets default resolution of image. |
