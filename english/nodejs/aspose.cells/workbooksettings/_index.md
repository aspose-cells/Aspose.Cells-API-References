---
title: "WorkbookSettings"
linktitle: "WorkbookSettings"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents all settings of the workbook."
type: docs
weight: 4720
url: /nodejs/aspose.cells/workbooksettings/
---

## WorkbookSettings class

Represents all settings of the workbook.

## Methods

| Name | Description |
| --- | --- |
| [dispose()](#dispose) | Releases resources. |
| [getAuthor()](#getauthor) | Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check th |
| [getAutoCompressPictures()](#getautocompresspictures) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [getAutoRecover()](#getautorecover) | Indicates whether the file is marked for auto-recovery. |
| [getBuildVersion()](#getbuildversion) | Specifies the incremental public release of the application. |
| [getCheckCompatibility()](#getcheckcompatibility) | Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Ex |
| [getCheckCustomNumberFormat()](#getcheckcustomnumberformat) | Indicates whether checking custom number format when setting Style.Custom. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [getCompliance()](#getcompliance) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is Oox |
| [getCrashSave()](#getcrashsave) | indicates whether the application last saved the workbook file after a crash. |
| [getDataExtractLoad()](#getdataextractload) | indicates whether the application last opened the workbook for data recovery. |
| [getDate1904()](#getdate1904) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [getDefaultImageResolution()](#getdefaultimageresolution) |  |
| [getDefaultStyleSettings()](#getdefaultstylesettings) | Gets the settings for default values of style-related properties for this workbook. |
| [getDiscardImageEditData()](#getdiscardimageeditdata) |  |
| [getDisplayDrawingObjects()](#getdisplaydrawingobjects) | Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer co |
| [getEnableMacros()](#getenablemacros) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [getFirstVisibleTab()](#getfirstvisibletab) | Gets or sets the first visible worksheet tab. |
| [getFormulaSettings()](#getformulasettings) | Gets the settings for formula-related features. |
| [getGlobalizationSettings()](#getglobalizationsettings) | Gets and sets the globalization settings. |
| [getHidePivotFieldList()](#gethidepivotfieldlist) | Gets and sets whether hide the field list for the PivotTable. |
| [getLanguageCode()](#getlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [getLocale()](#getlocale) | Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set. |
| [getMaxColumn()](#getmaxcolumn) | Gets the max column index, zero-based. Returns 255 if the file format is Excel97-2003; |
| [getMaxRow()](#getmaxrow) | Gets the max row index, zero-based. Returns 65535 if the file format is Excel97-2003; |
| [getMaxRowsOfSharedFormula()](#getmaxrowsofsharedformula) | Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Exc |
| [getMaxUniqueItemsPerField()](#getmaxuniqueitemsperfield) |  |
| [getMemorySetting()](#getmemorysetting) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets b |
| [getNumberDecimalSeparator()](#getnumberdecimalseparator) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Re |
| [getNumberGroupSeparator()](#getnumbergroupseparator) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the  |
| [getPaperSize()](#getpapersize) | Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no  |
| [getPassword()](#getpassword) | Represents Workbook file encryption password. |
| [getPropertiesFollowChartPoint()](#getpropertiesfollowchartpoint) |  |
| [getProtectionType()](#getprotectiontype) | Gets the protection type of the workbook. The value of the property is ProtectionType integer constant. |
| [getQuotePrefixToStyle()](#getquoteprefixtostyle) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark  |
| [getRegion()](#getregion) | Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant. |
| [getRemovePersonalInformation()](#getremovepersonalinformation) | True if personal information can be removed from the specified workbook. |
| [getRepairLoad()](#getrepairload) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [getResourceProvider()](#getresourceprovider) | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [getShapeDisplayType()](#getshapedisplaytype) | The value of the property is ShapeDisplayType integer constant. |
| [getShared()](#getshared) | Gets or sets a value that indicates whether the Workbook is shared. The default value is false. |
| [getSheetTabBarWidth()](#getsheettabbarwidth) | Width of worksheet tab bar (in 1/1000 of window width). |
| [getShowTabs()](#getshowtabs) | Get or sets a value whether the Workbook tabs are displayed. The default value is true. |
| [getSignificantDigits()](#getsignificantdigits) | Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits. Only could be 15 or  |
| [getSignificantDigitsType()](#getsignificantdigitstype) | The value of the property is SignificantDigitsType integer constant. |
| [getSmartTagOptions()](#getsmarttagoptions) |  |
| [getStreamProvider()](#getstreamprovider) | Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use Resource |
| [getThemeFont(type)](#getthemefont) | Gets the default theme font name. |
| [getUpdateAdjacentCellsBorder()](#getupdateadjacentcellsborder) | Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell  |
| [getUpdateLinksType()](#getupdatelinkstype) | Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integ |
| [getWindowHeight()](#getwindowheight) | The height of the window, in unit of point. |
| [getWindowHeightCM()](#getwindowheightcm) | The height of the window, in unit of centimeter. |
| [getWindowHeightInch()](#getwindowheightinch) | The height of the window, in unit of inch. |
| [getWindowLeft()](#getwindowleft) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [getWindowLeftCM()](#getwindowleftcm) | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [getWindowLeftInch()](#getwindowleftinch) | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [getWindowTop()](#getwindowtop) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [getWindowTopCM()](#getwindowtopcm) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [getWindowTopInch()](#getwindowtopinch) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [getWindowWidth()](#getwindowwidth) | The width of the window, in unit of point. |
| [getWindowWidthCM()](#getwindowwidthcm) | The width of the window, in unit of centimeter. |
| [getWindowWidthInch()](#getwindowwidthinch) | The width of the window, in unit of inch. |
| [getWpsCompatibility()](#getwpscompatibility) |  |
| [getWriteProtection()](#getwriteprotection) | Provides access to the workbook write protection options. |
| [isDefaultEncrypted()](#isdefaultencrypted) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The |
| [isEncrypted()](#isencrypted) | Gets a value that indicates whether a password is required to open this workbook. |
| [isHScrollBarVisible()](#ishscrollbarvisible) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default valu |
| [isHidden()](#ishidden) | Indicates whether this workbook is hidden. |
| [isMinimized()](#isminimized) | Represents whether the generated spreadsheet will be opened Minimized. |
| [isProtected()](#isprotected) | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isVScrollBarVisible()](#isvscrollbarvisible) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value  |
| [setAuthor()](#setauthor) | Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check th |
| [setAutoCompressPictures()](#setautocompresspictures) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [setAutoRecover()](#setautorecover) | Indicates whether the file is marked for auto-recovery. |
| [setBuildVersion()](#setbuildversion) | Specifies the incremental public release of the application. |
| [setCheckCompatibility()](#setcheckcompatibility) | Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Ex |
| [setCheckCustomNumberFormat()](#setcheckcustomnumberformat) | Indicates whether checking custom number format when setting Style.Custom. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [setCompliance()](#setcompliance) | Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is Oox |
| [setCrashSave()](#setcrashsave) | indicates whether the application last saved the workbook file after a crash. |
| [setDataExtractLoad()](#setdataextractload) | indicates whether the application last opened the workbook for data recovery. |
| [setDate1904()](#setdate1904) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [setDefaultEncrypted()](#setdefaultencrypted) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The |
| [setDefaultImageResolution()](#setdefaultimageresolution) |  |
| [setDiscardImageEditData()](#setdiscardimageeditdata) |  |
| [setDisplayDrawingObjects()](#setdisplaydrawingobjects) | Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer co |
| [setEnableMacros()](#setenablemacros) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [setFirstVisibleTab()](#setfirstvisibletab) | Gets or sets the first visible worksheet tab. |
| [setGlobalizationSettings()](#setglobalizationsettings) | Gets and sets the globalization settings. |
| [setHScrollBarVisible()](#sethscrollbarvisible) | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default valu |
| [setHidden()](#sethidden) | Indicates whether this workbook is hidden. |
| [setHidePivotFieldList()](#sethidepivotfieldlist) | Gets and sets whether hide the field list for the PivotTable. |
| [setLanguageCode()](#setlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [setLocale()](#setlocale) | Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set. |
| [setMaxRowsOfSharedFormula()](#setmaxrowsofsharedformula) | Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Exc |
| [setMaxUniqueItemsPerField()](#setmaxuniqueitemsperfield) |  |
| [setMemorySetting()](#setmemorysetting) | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets b |
| [setMinimized()](#setminimized) | Represents whether the generated spreadsheet will be opened Minimized. |
| [setNumberDecimalSeparator()](#setnumberdecimalseparator) | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Re |
| [setNumberGroupSeparator()](#setnumbergroupseparator) | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the  |
| [setPageOrientationType(pageOrientationType)](#setpageorientationtype) | Set the type of print orientation for the whole workbook. |
| [setPaperSize()](#setpapersize) | Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no  |
| [setPassword()](#setpassword) | Represents Workbook file encryption password. |
| [setPropertiesFollowChartPoint()](#setpropertiesfollowchartpoint) |  |
| [setQuotePrefixToStyle()](#setquoteprefixtostyle) | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark  |
| [setRegion()](#setregion) | Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant. |
| [setRemovePersonalInformation()](#setremovepersonalinformation) | True if personal information can be removed from the specified workbook. |
| [setRepairLoad()](#setrepairload) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [setResourceProvider()](#setresourceprovider) | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [setShapeDisplayType()](#setshapedisplaytype) | The value of the property is ShapeDisplayType integer constant. |
| [setShared()](#setshared) | Gets or sets a value that indicates whether the Workbook is shared. The default value is false. |
| [setSheetTabBarWidth()](#setsheettabbarwidth) | Width of worksheet tab bar (in 1/1000 of window width). |
| [setShowTabs()](#setshowtabs) | Get or sets a value whether the Workbook tabs are displayed. The default value is true. |
| [setSignificantDigits()](#setsignificantdigits) | Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits. Only could be 15 or  |
| [setSignificantDigitsType()](#setsignificantdigitstype) | The value of the property is SignificantDigitsType integer constant. |
| [setStreamProvider()](#setstreamprovider) | Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use Resource |
| [setUpdateAdjacentCellsBorder()](#setupdateadjacentcellsborder) | Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell  |
| [setUpdateLinksType()](#setupdatelinkstype) | Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integ |
| [setVScrollBarVisible()](#setvscrollbarvisible) | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value  |
| [setWindowHeight()](#setwindowheight) | The height of the window, in unit of point. |
| [setWindowHeightCM()](#setwindowheightcm) | The height of the window, in unit of centimeter. |
| [setWindowHeightInch()](#setwindowheightinch) | The height of the window, in unit of inch. |
| [setWindowLeft()](#setwindowleft) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [setWindowLeftCM()](#setwindowleftcm) | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [setWindowLeftInch()](#setwindowleftinch) | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [setWindowTop()](#setwindowtop) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [setWindowTopCM()](#setwindowtopcm) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [setWindowTopInch()](#setwindowtopinch) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [setWindowWidth()](#setwindowwidth) | The width of the window, in unit of point. |
| [setWindowWidthCM()](#setwindowwidthcm) | The width of the window, in unit of centimeter. |
| [setWindowWidthInch()](#setwindowwidthinch) | The width of the window, in unit of inch. |
| [setWpsCompatibility()](#setwpscompatibility) |  |

### dispose() {#dispose}

Releases resources.

### getAuthor() {#getauthor}

Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check the user of Environment.

### getAutoCompressPictures() {#getautocompresspictures}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

### getAutoRecover() {#getautorecover}

Indicates whether the file is marked for auto-recovery.

### getBuildVersion() {#getbuildversion}

Specifies the incremental public release of the application.

### getCheckCompatibility() {#getcheckcompatibility}

Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Excel97-2003 xls or xlt files.

### getCheckCustomNumberFormat() {#getcheckcustomnumberformat}

Indicates whether checking custom number format when setting Style.Custom.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### getCompliance() {#getcompliance}

Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is OoxmlCompliance integer constant. Only for .xlsx files.

### getCrashSave() {#getcrashsave}

indicates whether the application last saved the workbook file after a crash.

### getDataExtractLoad() {#getdataextractload}

indicates whether the application last opened the workbook for data recovery.

### getDate1904() {#getdate1904}

Gets or sets a value which represents if the workbook uses the 1904 date system.

### getDefaultImageResolution() {#getdefaultimageresolution}

### getDefaultStyleSettings() {#getdefaultstylesettings}

Gets the settings for default values of style-related properties for this workbook.

### getDiscardImageEditData() {#getdiscardimageeditdata}

### getDisplayDrawingObjects() {#getdisplaydrawingobjects}

Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer constant.

### getEnableMacros() {#getenablemacros}

Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

### getFirstVisibleTab() {#getfirstvisibletab}

Gets or sets the first visible worksheet tab.

### getFormulaSettings() {#getformulasettings}

Gets the settings for formula-related features.

### getGlobalizationSettings() {#getglobalizationsettings}

Gets and sets the globalization settings.

### getHidePivotFieldList() {#gethidepivotfieldlist}

Gets and sets whether hide the field list for the PivotTable.

### getLanguageCode() {#getlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### getLocale() {#getlocale}

Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set.

### getMaxColumn() {#getmaxcolumn}

Gets the max column index, zero-based. Returns 255 if the file format is Excel97-2003;

### getMaxRow() {#getmaxrow}

Gets the max row index, zero-based. Returns 65535 if the file format is Excel97-2003;

### getMaxRowsOfSharedFormula() {#getmaxrowsofsharedformula}

Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Excel 2013.

### getMaxUniqueItemsPerField() {#getmaxuniqueitemsperfield}

### getMemorySetting() {#getmemorysetting}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. The value of the property is MemorySetting integer constant.

### getNumberDecimalSeparator() {#getnumberdecimalseparator}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

### getNumberGroupSeparator() {#getnumbergroupseparator}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

### getPaperSize() {#getpapersize}

Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no setting about paper size,MS Excel will use default printer's setting.

### getPassword() {#getpassword}

Represents Workbook file encryption password.

### getPropertiesFollowChartPoint() {#getpropertiesfollowchartpoint}

### getProtectionType() {#getprotectiontype}

Gets the protection type of the workbook. The value of the property is ProtectionType integer constant.

### getQuotePrefixToStyle() {#getquoteprefixtostyle}

Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark ) to the cell

### getRegion() {#getregion}

Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant.

### getRemovePersonalInformation() {#getremovepersonalinformation}

True if personal information can be removed from the specified workbook.

### getRepairLoad() {#getrepairload}

Indicates whether the application last opened the workbook in safe or repair mode.

### getResourceProvider() {#getresourceprovider}

Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

### getShapeDisplayType() {#getshapedisplaytype}

The value of the property is ShapeDisplayType integer constant.

### getShared() {#getshared}

Gets or sets a value that indicates whether the Workbook is shared. The default value is false.

### getSheetTabBarWidth() {#getsheettabbarwidth}

Width of worksheet tab bar (in 1/1000 of window width).

### getShowTabs() {#getshowtabs}

Get or sets a value whether the Workbook tabs are displayed. The default value is true.

### getSignificantDigits() {#getsignificantdigits}

Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits. Only could be 15 or 17 now.

### getSignificantDigitsType() {#getsignificantdigitstype}

The value of the property is SignificantDigitsType integer constant.

### getSmartTagOptions() {#getsmarttagoptions}

### getStreamProvider() {#getstreamprovider}

Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### getThemeFont(type) {#getthemefont}

Gets the default theme font name.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | FontSchemeType |

**Returns:** String — `String`

### getUpdateAdjacentCellsBorder() {#getupdateadjacentcellsborder}

Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### getUpdateLinksType() {#getupdatelinkstype}

Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integer constant.

### getWindowHeight() {#getwindowheight}

The height of the window, in unit of point.

### getWindowHeightCM() {#getwindowheightcm}

The height of the window, in unit of centimeter.

### getWindowHeightInch() {#getwindowheightinch}

The height of the window, in unit of inch.

### getWindowLeft() {#getwindowleft}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

### getWindowLeftCM() {#getwindowleftcm}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

### getWindowLeftInch() {#getwindowleftinch}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

### getWindowTop() {#getwindowtop}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

### getWindowTopCM() {#getwindowtopcm}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

### getWindowTopInch() {#getwindowtopinch}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

### getWindowWidth() {#getwindowwidth}

The width of the window, in unit of point.

### getWindowWidthCM() {#getwindowwidthcm}

The width of the window, in unit of centimeter.

### getWindowWidthInch() {#getwindowwidthinch}

The width of the window, in unit of inch.

### getWpsCompatibility() {#getwpscompatibility}

### getWriteProtection() {#getwriteprotection}

Provides access to the workbook write protection options.

### isDefaultEncrypted() {#isdefaultencrypted}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The default value is false now. It's same as MS Excel 2013.

### isEncrypted() {#isencrypted}

Gets a value that indicates whether a password is required to open this workbook.

### isHScrollBarVisible() {#ishscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default value is true.

### isHidden() {#ishidden}

Indicates whether this workbook is hidden.

### isMinimized() {#isminimized}

Represents whether the generated spreadsheet will be opened Minimized.

### isProtected() {#isprotected}

Gets a value that indicates whether the structure or window of the Workbook is protected.

### isVScrollBarVisible() {#isvscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value is true.

### setAuthor() {#setauthor}

Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check the user of Environment.

### setAutoCompressPictures() {#setautocompresspictures}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

### setAutoRecover() {#setautorecover}

Indicates whether the file is marked for auto-recovery.

### setBuildVersion() {#setbuildversion}

Specifies the incremental public release of the application.

### setCheckCompatibility() {#setcheckcompatibility}

Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Excel97-2003 xls or xlt files.

### setCheckCustomNumberFormat() {#setcheckcustomnumberformat}

Indicates whether checking custom number format when setting Style.Custom.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### setCompliance() {#setcompliance}

Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is OoxmlCompliance integer constant. Only for .xlsx files.

### setCrashSave() {#setcrashsave}

indicates whether the application last saved the workbook file after a crash.

### setDataExtractLoad() {#setdataextractload}

indicates whether the application last opened the workbook for data recovery.

### setDate1904() {#setdate1904}

Gets or sets a value which represents if the workbook uses the 1904 date system.

### setDefaultEncrypted() {#setdefaultencrypted}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The default value is false now. It's same as MS Excel 2013.

### setDefaultImageResolution() {#setdefaultimageresolution}

### setDiscardImageEditData() {#setdiscardimageeditdata}

### setDisplayDrawingObjects() {#setdisplaydrawingobjects}

Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer constant.

### setEnableMacros() {#setenablemacros}

Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

### setFirstVisibleTab() {#setfirstvisibletab}

Gets or sets the first visible worksheet tab.

### setGlobalizationSettings() {#setglobalizationsettings}

Gets and sets the globalization settings.

### setHScrollBarVisible() {#sethscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default value is true.

### setHidden() {#sethidden}

Indicates whether this workbook is hidden.

### setHidePivotFieldList() {#sethidepivotfieldlist}

Gets and sets whether hide the field list for the PivotTable.

### setLanguageCode() {#setlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### setLocale() {#setlocale}

Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set.

### setMaxRowsOfSharedFormula() {#setmaxrowsofsharedformula}

Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Excel 2013.

### setMaxUniqueItemsPerField() {#setmaxuniqueitemsperfield}

### setMemorySetting() {#setmemorysetting}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. The value of the property is MemorySetting integer constant.

### setMinimized() {#setminimized}

Represents whether the generated spreadsheet will be opened Minimized.

### setNumberDecimalSeparator() {#setnumberdecimalseparator}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

### setNumberGroupSeparator() {#setnumbergroupseparator}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

### setPageOrientationType(pageOrientationType) {#setpageorientationtype}

Set the type of print orientation for the whole workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | Number | PageOrientationType |

### setPaperSize() {#setpapersize}

Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no setting about paper size,MS Excel will use default printer's setting.

### setPassword() {#setpassword}

Represents Workbook file encryption password.

### setPropertiesFollowChartPoint() {#setpropertiesfollowchartpoint}

### setQuotePrefixToStyle() {#setquoteprefixtostyle}

Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark ) to the cell

### setRegion() {#setregion}

Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant.

### setRemovePersonalInformation() {#setremovepersonalinformation}

True if personal information can be removed from the specified workbook.

### setRepairLoad() {#setrepairload}

Indicates whether the application last opened the workbook in safe or repair mode.

### setResourceProvider() {#setresourceprovider}

Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

### setShapeDisplayType() {#setshapedisplaytype}

The value of the property is ShapeDisplayType integer constant.

### setShared() {#setshared}

Gets or sets a value that indicates whether the Workbook is shared. The default value is false.

### setSheetTabBarWidth() {#setsheettabbarwidth}

Width of worksheet tab bar (in 1/1000 of window width).

### setShowTabs() {#setshowtabs}

Get or sets a value whether the Workbook tabs are displayed. The default value is true.

### setSignificantDigits() {#setsignificantdigits}

Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits. Only could be 15 or 17 now.

### setSignificantDigitsType() {#setsignificantdigitstype}

The value of the property is SignificantDigitsType integer constant.

### setStreamProvider() {#setstreamprovider}

Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### setUpdateAdjacentCellsBorder() {#setupdateadjacentcellsborder}

Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### setUpdateLinksType() {#setupdatelinkstype}

Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integer constant.

### setVScrollBarVisible() {#setvscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value is true.

### setWindowHeight() {#setwindowheight}

The height of the window, in unit of point.

### setWindowHeightCM() {#setwindowheightcm}

The height of the window, in unit of centimeter.

### setWindowHeightInch() {#setwindowheightinch}

The height of the window, in unit of inch.

### setWindowLeft() {#setwindowleft}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

### setWindowLeftCM() {#setwindowleftcm}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

### setWindowLeftInch() {#setwindowleftinch}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

### setWindowTop() {#setwindowtop}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

### setWindowTopCM() {#setwindowtopcm}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

### setWindowTopInch() {#setwindowtopinch}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

### setWindowWidth() {#setwindowwidth}

The width of the window, in unit of point.

### setWindowWidthCM() {#setwindowwidthcm}

The width of the window, in unit of centimeter.

### setWindowWidthInch() {#setwindowwidthinch}

The width of the window, in unit of inch.

### setWpsCompatibility() {#setwpscompatibility}
