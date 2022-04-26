---
title: WorkbookSettings
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 6470
url: /net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Represents all settings of the workbook.

```csharp
public class WorkbookSettings : IDisposable
```

## Properties

| Name | Description |
| --- | --- |
| [Author](author) { get; set; } | Gets and sets the author of the file. |
| [AutoCompressPictures](autocompresspictures) { get; set; } | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [AutoRecover](autorecover) { get; set; } | Indicates whether the file is mark for auto-recovery. |
| [BuildVersion](buildversion) { get; set; } | Specifies the incremental public release of the application. |
| [CheckCompatibility](checkcompatibility) { get; set; } | Indicates whether check compatibility with earlier versions when saving workbook. |
| [CheckCustomNumberFormat](checkcustomnumberformat) { get; set; } | Indicates whether checking custom number format when setting Style.Custom. |
| [CheckExcelRestriction](checkexcelrestriction) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [Compliance](compliance) { get; set; } | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [CrashSave](crashsave) { get; set; } | indicates whether the application last saved the workbook file after a crash. |
| [CultureInfo](cultureinfo) { get; set; } | Gets or sets the system culture info. |
| [DataExtractLoad](dataextractload) { get; set; } | indicates whether the application last opened the workbook for data recovery. |
| [Date1904](date1904) { get; set; } | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [DisplayDrawingObjects](displaydrawingobjects) { get; set; } | Indicates whether and how to show objects in the workbook. |
| [EnableMacros](enablemacros) { get; set; } | Enable macros; |
| [FirstVisibleTab](firstvisibletab) { get; set; } | Gets or sets the first visible worksheet tab. |
| [FormulaSettings](formulasettings) { get; } | Gets the settings for formula-related features. |
| [GlobalizationSettings](globalizationsettings) { get; set; } | Gets and sets the globalization settings. |
| [HidePivotFieldList](hidepivotfieldlist) { get; set; } | Gets and sets whether hide the field list for the PivotTable. |
| [IsDefaultEncrypted](isdefaultencrypted) { get; set; } | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [IsEncrypted](isencrypted) { get; } | Gets a value that indicates whether a password is required to open this workbook. |
| [IsHidden](ishidden) { get; set; } | Indicates whether this workbook is hidden. |
| [IsHScrollBarVisible](ishscrollbarvisible) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [IsMinimized](isminimized) { get; set; } | Represents whether the generated spreadsheet will be opened Minimized. |
| [IsProtected](isprotected) { get; } | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [IsVScrollBarVisible](isvscrollbarvisible) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [LanguageCode](languagecode) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [MaxColumn](maxcolumn) { get; } | Gets the max column index, zero-based. |
| [MaxRow](maxrow) { get; } | Gets the max row index, zero-based. |
| [MaxRowsOfSharedFormula](maxrowsofsharedformula) { get; set; } | Gets and sets the max row number of shared formula. |
| [MemorySetting](memorysetting) { get; set; } | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [NumberDecimalSeparator](numberdecimalseparator) { get; set; } | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [NumberGroupSeparator](numbergroupseparator) { get; set; } | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [PaperSize](papersize) { get; set; } | Gets and sets the default print paper size. |
| [Password](password) { get; set; } | Represents Workbook file encryption password. |
| [ProtectionType](protectiontype) { get; } | Gets the protection type of the workbook. |
| [QuotePrefixToStyle](quoteprefixtostyle) { get; set; } | Indicates whether setting [`QuotePrefix`](../style/quoteprefix) property when entering the string value(which starts with single quote mark ) to the cell |
| [Region](region) { get; set; } | Gets or sets the regional settings for workbook. |
| [RemovePersonalInformation](removepersonalinformation) { get; set; } | True if personal information can be removed from the specified workbook. |
| [RepairLoad](repairload) { get; set; } | Indicates whether the application last opened the workbook in safe or repair mode. |
| [ResourceProvider](resourceprovider) { get; set; } | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [Shared](shared) { get; set; } | Gets or sets a value that indicates whether the Workbook is shared. |
| [SheetTabBarWidth](sheettabbarwidth) { get; set; } | Width of worksheet tab bar (in 1/1000 of window width). |
| [ShowTabs](showtabs) { get; set; } | Get or sets a value whether the Workbook tabs are displayed. |
| [SignificantDigits](significantdigits) { get; set; } | Gets and sets the number of significant digits. The default value is [`SignificantDigits`](../cellshelper/significantdigits). |
| [UpdateAdjacentCellsBorder](updateadjacentcellsborder) { get; set; } | Indicates whether update adjacent cells' border. |
| [UpdateLinksType](updatelinkstype) { get; set; } | Gets and sets how updates external links when the workbook is opened. |
| [WarningCallback](warningcallback) { get; set; } | Gets or sets warning callback. |
| [WindowHeight](windowheight) { get; set; } | The height of the window, in unit of point. |
| [WindowHeightCM](windowheightcm) { get; set; } | The height of the window, in unit of centimeter. |
| [WindowHeightInch](windowheightinch) { get; set; } | The height of the window, in unit of inch. |
| [WindowLeft](windowleft) { get; set; } | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [WindowLeftCM](windowleftcm) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [WindowLeftInch](windowleftinch) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [WindowTop](windowtop) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [WindowTopCM](windowtopcm) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [WindowTopInch](windowtopinch) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [WindowWidth](windowwidth) { get; set; } | The width of the window, in unit of point. |
| [WindowWidthCM](windowwidthcm) { get; set; } | The width of the window, in unit of centimeter. |
| [WindowWidthInch](windowwidthinch) { get; set; } | The width of the window, in unit of inch. |
| [WriteProtection](writeprotection) { get; } | Provides access to the workbook write protection options. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](dispose)() | Releases resources. |
| [GetThemeFont](getthemefont)(FontSchemeType) | Gets the default theme font name. |
| [SetPageOrientationType](setpageorientationtype)(PageOrientationType) | Set the type of print orientation for the whole workbook. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//do your business

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'do your business
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
