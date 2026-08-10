---
title: "WorkbookSettings Class"
linktitle: "WorkbookSettings"
articleTitle: "WorkbookSettings"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents all settings of the workbook."
type: docs
weight: 7590
url: /php/aspose.cells/workbooksettings/
---

## WorkbookSettings class

Represents all settings of the workbook.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [StreamProvider](#streamprovider) | IStreamProvider | Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use Resource |
| [ResourceProvider](#resourceprovider) | IStreamProvider | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [Author](#author) | String | Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check th |
| [CheckCustomNumberFormat](#checkcustomnumberformat) | boolean | Indicates whether checking custom number format when setting Style.Custom. |
| [EnableMacros](#enablemacros) | boolean | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [Date1904](#date1904) | boolean | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [ProtectionType](#protectiontype) | Number | Gets the protection type of the workbook. The value of the property is ProtectionType integer constant. |
| [DisplayDrawingObjects](#displaydrawingobjects) | Number | Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer co |
| [SheetTabBarWidth](#sheettabbarwidth) | Number | Width of worksheet tab bar (in 1/1000 of window width). |
| [ShowTabs](#showtabs) | boolean | Get or sets a value whether the Workbook tabs are displayed. The default value is true. |
| [FirstVisibleTab](#firstvisibletab) | Number | Gets or sets the first visible worksheet tab. |
| [IsHScrollBarVisible](#ishscrollbarvisible) | boolean | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default valu |
| [IsVScrollBarVisible](#isvscrollbarvisible) | boolean | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value  |
| [Shared](#shared) | boolean | Gets or sets a value that indicates whether the Workbook is shared. The default value is false. |
| [LanguageCode](#languagecode) | Number | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [Region](#region) | Number | Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant. 1. Regional  |
| [Locale](#locale) | Locale | Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set. |
| [GlobalizationSettings](#globalizationsettings) | GlobalizationSettings | Gets and sets the globalization settings. |
| [NumberDecimalSeparator](#numberdecimalseparator) | char | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Re |
| [NumberGroupSeparator](#numbergroupseparator) | char | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the  |
| [Password](#password) | String | Represents Workbook file encryption password. |
| [WriteProtection](#writeprotection) | WriteProtection | Provides access to the workbook write protection options. |
| [IsEncrypted](#isencrypted) | boolean | Gets a value that indicates whether a password is required to open this workbook. |
| [IsProtected](#isprotected) | boolean | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [IsDefaultEncrypted](#isdefaultencrypted) | boolean | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The |
| [IsMinimized](#isminimized) | boolean | Represents whether the generated spreadsheet will be opened Minimized. |
| [IsHidden](#ishidden) | boolean | Indicates whether this workbook is hidden. |
| [AutoCompressPictures](#autocompresspictures) | boolean | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [RemovePersonalInformation](#removepersonalinformation) | boolean | True if personal information can be removed from the specified workbook. |
| [ShapeDisplayType](#shapedisplaytype) | Number | The value of the property is ShapeDisplayType integer constant. |
| [HidePivotFieldList](#hidepivotfieldlist) | boolean | Gets and sets whether hide the field list for the PivotTable. |
| [MaxUniqueItemsPerField](#maxuniqueitemsperfield) | Number |  |
| [UpdateLinksType](#updatelinkstype) | Number | Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integ |
| [MaxRow](#maxrow) | Number | Gets the max row index, zero-based. Returns 65535 if the file format is Excel97-2003; |
| [MaxColumn](#maxcolumn) | Number | Gets the max column index, zero-based. Returns 255 if the file format is Excel97-2003; |
| [SmartTagOptions](#smarttagoptions) | SmartTagOptions |  |
| [DefaultStyleSettings](#defaultstylesettings) | DefaultStyleSettings | Gets the settings for default values of style-related properties for this workbook. |
| [WindowLeft](#windowleft) | Number | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [WindowLeftInch](#windowleftinch) | Number | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [WindowLeftCM](#windowleftcm) | Number | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [WindowTop](#windowtop) | Number | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [WindowTopInch](#windowtopinch) | Number | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [WindowTopCM](#windowtopcm) | Number | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [WindowWidth](#windowwidth) | Number | The width of the window, in unit of point. |
| [WindowWidthInch](#windowwidthinch) | Number | The width of the window, in unit of inch. |
| [WindowWidthCM](#windowwidthcm) | Number | The width of the window, in unit of centimeter. |
| [WindowHeight](#windowheight) | Number | The height of the window, in unit of point. |
| [WindowHeightInch](#windowheightinch) | Number | The height of the window, in unit of inch. |
| [WindowHeightCM](#windowheightcm) | Number | The height of the window, in unit of centimeter. |
| [UpdateAdjacentCellsBorder](#updateadjacentcellsborder) | boolean | Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell  |
| [SignificantDigits](#significantdigits) | Number | Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits . Only could be 15 or |
| [SignificantDigitsType](#significantdigitstype) | Number | The value of the property is SignificantDigitsType integer constant. |
| [CheckCompatibility](#checkcompatibility) | boolean | Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Ex |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [AutoRecover](#autorecover) | boolean | Indicates whether the file is marked for auto-recovery. |
| [CrashSave](#crashsave) | boolean | indicates whether the application last saved the workbook file after a crash. |
| [DataExtractLoad](#dataextractload) | boolean | indicates whether the application last opened the workbook for data recovery. |
| [RepairLoad](#repairload) | boolean | Indicates whether the application last opened the workbook in safe or repair mode. |
| [BuildVersion](#buildversion) | String | Specifies the incremental public release of the application. |
| [MemorySetting](#memorysetting) | Number | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets b |
| [PaperSize](#papersize) | Number | Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no  |
| [MaxRowsOfSharedFormula](#maxrowsofsharedformula) | Number | Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Exc |
| [Compliance](#compliance) | Number | Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is Oox |
| [QuotePrefixToStyle](#quoteprefixtostyle) | boolean | Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark  |
| [FormulaSettings](#formulasettings) | FormulaSettings | Gets the settings for formula-related features. |
| [PropertiesFollowChartPoint](#propertiesfollowchartpoint) | boolean |  |
| [DiscardImageEditData](#discardimageeditdata) | boolean |  |
| [DefaultImageResolution](#defaultimageresolution) | Number |  |
| [WpsCompatibility](#wpscompatibility) | boolean |  |

## Methods

| Name | Description |
| --- | --- |
| [dispose](#dispose) | Releases resources. |
| [getThemeFont](#getthemefont) | Gets the default theme font name. |
| [setPageOrientationType](#setpageorientationtype) | Set the type of print orientation for the whole workbook. |

### WorkbookSettings.StreamProvider property {#streamprovider}

Gets and sets the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** IStreamProvider

### WorkbookSettings.ResourceProvider property {#resourceprovider}

Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

**Type:** IStreamProvider

### WorkbookSettings.Author property {#author}

Gets and sets the author of the file. It''s not set, check BuiltInDocumentPropertyCollection.Author first, then check the user of Environment.

**Type:** String

### WorkbookSettings.CheckCustomNumberFormat property {#checkcustomnumberformat}

Indicates whether checking custom number format when setting Style.Custom.

**Type:** boolean

### WorkbookSettings.EnableMacros property {#enablemacros}

Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

**Type:** boolean

### WorkbookSettings.Date1904 property {#date1904}

Gets or sets a value which represents if the workbook uses the 1904 date system.

**Type:** boolean

### WorkbookSettings.ProtectionType property {#protectiontype}

Gets the protection type of the workbook. The value of the property is ProtectionType integer constant.

**Type:** Number

### WorkbookSettings.DisplayDrawingObjects property {#displaydrawingobjects}

Indicates whether and how to show objects in the workbook. The value of the property is DisplayDrawingObjects integer constant.

**Type:** Number

### WorkbookSettings.SheetTabBarWidth property {#sheettabbarwidth}

Width of worksheet tab bar (in 1/1000 of window width).

**Type:** Number

### WorkbookSettings.ShowTabs property {#showtabs}

Get or sets a value whether the Workbook tabs are displayed. The default value is true.

**Type:** boolean

### WorkbookSettings.FirstVisibleTab property {#firstvisibletab}

Gets or sets the first visible worksheet tab.

**Type:** Number

### WorkbookSettings.IsHScrollBarVisible property {#ishscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default value is true.

**Type:** boolean

### WorkbookSettings.IsVScrollBarVisible property {#isvscrollbarvisible}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value is true.

**Type:** boolean

### WorkbookSettings.Shared property {#shared}

Gets or sets a value that indicates whether the Workbook is shared. The default value is false.

**Type:** boolean

### WorkbookSettings.LanguageCode property {#languagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

**Type:** Number

### WorkbookSettings.Region property {#region}

Gets or sets the regional settings for workbook. The value of the property is CountryCode integer constant. 1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

**Type:** Number

### WorkbookSettings.Locale property {#locale}

Gets or sets the Locale used by this workbook. Returns null if neither Locale nor Region is set.

**Type:** Locale

### WorkbookSettings.GlobalizationSettings property {#globalizationsettings}

Gets and sets the globalization settings.

**Type:** GlobalizationSettings

### WorkbookSettings.NumberDecimalSeparator property {#numberdecimalseparator}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

**Type:** char

### WorkbookSettings.NumberGroupSeparator property {#numbergroupseparator}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

**Type:** char

### WorkbookSettings.Password property {#password}

Represents Workbook file encryption password.

**Type:** String

### WorkbookSettings.WriteProtection property {#writeprotection}

Provides access to the workbook write protection options.

**Type:** WriteProtection

### WorkbookSettings.IsEncrypted property {#isencrypted}

Gets a value that indicates whether a password is required to open this workbook.

**Type:** boolean

### WorkbookSettings.IsProtected property {#isprotected}

Gets a value that indicates whether the structure or window of the Workbook is protected.

**Type:** boolean

### WorkbookSettings.IsDefaultEncrypted property {#isdefaultencrypted}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The default value is false now. It's same as MS Excel 2013.

**Type:** boolean

### WorkbookSettings.IsMinimized property {#isminimized}

Represents whether the generated spreadsheet will be opened Minimized.

**Type:** boolean

### WorkbookSettings.IsHidden property {#ishidden}

Indicates whether this workbook is hidden.

**Type:** boolean

### WorkbookSettings.AutoCompressPictures property {#autocompresspictures}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

**Type:** boolean

### WorkbookSettings.RemovePersonalInformation property {#removepersonalinformation}

True if personal information can be removed from the specified workbook.

**Type:** boolean

### WorkbookSettings.ShapeDisplayType property {#shapedisplaytype}

The value of the property is ShapeDisplayType integer constant.

**Type:** Number

### WorkbookSettings.HidePivotFieldList property {#hidepivotfieldlist}

Gets and sets whether hide the field list for the PivotTable.

**Type:** boolean

### WorkbookSettings.MaxUniqueItemsPerField property {#maxuniqueitemsperfield}

**Type:** Number

### WorkbookSettings.UpdateLinksType property {#updatelinkstype}

Gets and sets how updates external links when the workbook is opened. The value of the property is UpdateLinksType integer constant.

**Type:** Number

### WorkbookSettings.MaxRow property {#maxrow}

Gets the max row index, zero-based. Returns 65535 if the file format is Excel97-2003;

**Type:** Number

### WorkbookSettings.MaxColumn property {#maxcolumn}

Gets the max column index, zero-based. Returns 255 if the file format is Excel97-2003;

**Type:** Number

### WorkbookSettings.SmartTagOptions property {#smarttagoptions}

**Type:** SmartTagOptions

### WorkbookSettings.DefaultStyleSettings property {#defaultstylesettings}

Gets the settings for default values of style-related properties for this workbook.

**Type:** DefaultStyleSettings

### WorkbookSettings.WindowLeft property {#windowleft}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

**Type:** Number

### WorkbookSettings.WindowLeftInch property {#windowleftinch}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

**Type:** Number

### WorkbookSettings.WindowLeftCM property {#windowleftcm}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

**Type:** Number

### WorkbookSettings.WindowTop property {#windowtop}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

**Type:** Number

### WorkbookSettings.WindowTopInch property {#windowtopinch}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

**Type:** Number

### WorkbookSettings.WindowTopCM property {#windowtopcm}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

**Type:** Number

### WorkbookSettings.WindowWidth property {#windowwidth}

The width of the window, in unit of point.

**Type:** Number

### WorkbookSettings.WindowWidthInch property {#windowwidthinch}

The width of the window, in unit of inch.

**Type:** Number

### WorkbookSettings.WindowWidthCM property {#windowwidthcm}

The width of the window, in unit of centimeter.

**Type:** Number

### WorkbookSettings.WindowHeight property {#windowheight}

The height of the window, in unit of point.

**Type:** Number

### WorkbookSettings.WindowHeightInch property {#windowheightinch}

The height of the window, in unit of inch.

**Type:** Number

### WorkbookSettings.WindowHeightCM property {#windowheightcm}

The height of the window, in unit of centimeter.

**Type:** Number

### WorkbookSettings.UpdateAdjacentCellsBorder property {#updateadjacentcellsborder}

Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Type:** boolean

### WorkbookSettings.SignificantDigits property {#significantdigits}

Gets and sets the number of significant digits. The default value is CellsHelper.SignificantDigits . Only could be 15 or 17 now.

**Type:** Number

### WorkbookSettings.SignificantDigitsType property {#significantdigitstype}

The value of the property is SignificantDigitsType integer constant.

**Type:** Number

### WorkbookSettings.CheckCompatibility property {#checkcompatibility}

Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Excel97-2003 xls or xlt files.

**Type:** boolean

### WorkbookSettings.CheckExcelRestriction property {#checkexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Type:** boolean

### WorkbookSettings.AutoRecover property {#autorecover}

Indicates whether the file is marked for auto-recovery.

**Type:** boolean

### WorkbookSettings.CrashSave property {#crashsave}

indicates whether the application last saved the workbook file after a crash.

**Type:** boolean

### WorkbookSettings.DataExtractLoad property {#dataextractload}

indicates whether the application last opened the workbook for data recovery.

**Type:** boolean

### WorkbookSettings.RepairLoad property {#repairload}

Indicates whether the application last opened the workbook in safe or repair mode.

**Type:** boolean

### WorkbookSettings.BuildVersion property {#buildversion}

Specifies the incremental public release of the application.

**Type:** String

### WorkbookSettings.MemorySetting property {#memorysetting}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. The value of the property is MemorySetting integer constant.

**Type:** Number

### WorkbookSettings.PaperSize property {#papersize}

Gets and sets the default print paper size. The value of the property is PaperSizeType integer constant. If there is no setting about paper size,MS Excel will use default printer's setting.

**Type:** Number

### WorkbookSettings.MaxRowsOfSharedFormula property {#maxrowsofsharedformula}

Gets and sets the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Excel 2013.

**Type:** Number

### WorkbookSettings.Compliance property {#compliance}

Specifies the OOXML version for the output document. The default value is Ecma376_2006. The value of the property is OoxmlCompliance integer constant. Only for .xlsx files.

**Type:** Number

### WorkbookSettings.QuotePrefixToStyle property {#quoteprefixtostyle}

Indicates whether setting Style.QuotePrefix property when entering the string value(which starts with single quote mark ) to the cell

**Type:** boolean

### WorkbookSettings.FormulaSettings property {#formulasettings}

Gets the settings for formula-related features.

**Type:** FormulaSettings

### WorkbookSettings.PropertiesFollowChartPoint property {#propertiesfollowchartpoint}

**Type:** boolean

### WorkbookSettings.DiscardImageEditData property {#discardimageeditdata}

**Type:** boolean

### WorkbookSettings.DefaultImageResolution property {#defaultimageresolution}

**Type:** Number

### WorkbookSettings.WpsCompatibility property {#wpscompatibility}

**Type:** boolean

### dispose() {#dispose}

Releases resources.

### getThemeFont(type) {#getthemefont}

Gets the default theme font name.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A FontSchemeType value. The scheme type of the font. |

### setPageOrientationType(pageOrientationType) {#setpageorientationtype}

Set the type of print orientation for the whole workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | Number | A PageOrientationType value. The page orientation type |
