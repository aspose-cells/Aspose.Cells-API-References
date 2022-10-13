---
title: WorkbookSettings
second_title: Aspose.Cells for .NET API Reference
description: Represents all settings of the workbook.
type: docs
weight: 6590
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
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Gets and sets the author of the file. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Indicates whether the file is mark for auto-recovery. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Specifies the incremental public release of the application. |
| [CalcMode](../../aspose.cells/workbooksettings/calcmode) { get; set; } | (**Obsolete.**) It specifies whether to calculate formulas manually, automatically or automatically except for multiple table operations. |
| [CalcStackSize](../../aspose.cells/workbooksettings/calcstacksize) { get; set; } | (**Obsolete.**) Specifies the stack size for calculating cells recursively. The large value for this size will give better performance when there are lots of cells need to be calculated recursively. On the other hand, larger value will raise the risk of StackOverflowException. If user gets StackOverflowException when calculating formulas, this value should be decreased. |
| [CalculationId](../../aspose.cells/workbooksettings/calculationid) { get; set; } | (**Obsolete.**) Specifies the version of the calculation engine used to calculate values in the workbook. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Indicates whether check compatibility with earlier versions when saving workbook. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Indicates whether checking custom number format when setting Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | indicates whether the application last saved the workbook file after a crash. |
| [CreateCalcChain](../../aspose.cells/workbooksettings/createcalcchain) { get; set; } | (**Obsolete.**) Whether creates calculated formulas chain. Default is false. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Gets or sets the system culture info. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | indicates whether the application last opened the workbook for data recovery. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Indicates whether and how to show objects in the workbook. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Enable macros; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Gets or sets the first visible worksheet tab. |
| [ForceFullCalculate](../../aspose.cells/workbooksettings/forcefullcalculate) { get; set; } | (**Obsolete.**) Fully calculates every time when a calculation is triggered. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Gets the settings for formula-related features. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Gets and sets the globalization settings. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Gets and sets whether hide the field list for the PivotTable. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Gets a value that indicates whether a password is required to open this workbook. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Indicates whether this workbook is hidden. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Represents whether the generated spreadsheet will be opened Minimized. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [Iteration](../../aspose.cells/workbooksettings/iteration) { get; set; } | (**Obsolete.**) Indicates whether enable iterative calculation to resolve circular references. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [MaxChange](../../aspose.cells/workbooksettings/maxchange) { get; set; } | (**Obsolete.**) Returns or sets the maximum number of change to resolve a circular reference. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Gets the max column index, zero-based. |
| [MaxIteration](../../aspose.cells/workbooksettings/maxiteration) { get; set; } | (**Obsolete.**) Returns or sets the maximum number of iterations to resolve a circular reference. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Gets the max row index, zero-based. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Gets and sets the max row number of shared formula. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Gets and sets the default print paper size. |
| [ParsingFormulaOnOpen](../../aspose.cells/workbooksettings/parsingformulaonopen) { get; set; } | (**Obsolete.**) Indicates whether parsing the formula when reading the file. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Represents Workbook file encryption password. |
| [PrecisionAsDisplayed](../../aspose.cells/workbooksettings/precisionasdisplayed) { get; set; } | (**Obsolete.**) True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Gets the protection type of the workbook. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Indicates whether setting [`QuotePrefix`](../style/quoteprefix) property when entering the string value(which starts with single quote mark ) to the cell |
| [RecalculateBeforeSave](../../aspose.cells/workbooksettings/recalculatebeforesave) { get; set; } | (**Obsolete.**) Indicates whether to recalculate before saving the document. |
| [ReCalculateOnOpen](../../aspose.cells/workbooksettings/recalculateonopen) { get; set; } | (**Obsolete.**) Indicates whether re-calculate all formulas on opening file. |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Gets or sets the regional settings for workbook. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | True if personal information can be removed from the specified workbook. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Indicates whether the application last opened the workbook in safe or repair mode. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Gets or sets a value that indicates whether the Workbook is shared. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Width of worksheet tab bar (in 1/1000 of window width). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Get or sets a value whether the Workbook tabs are displayed. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Gets and sets the number of significant digits. The default value is [`SignificantDigits`](../cellshelper/significantdigits). |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider) { get; set; } | (**Obsolete.**) Gets and sets the stream provider for external resource. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Indicates whether update adjacent cells' border. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Gets and sets how updates external links when the workbook is opened. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Gets or sets warning callback. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | The height of the window, in unit of point. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | The height of the window, in unit of centimeter. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | The height of the window, in unit of inch. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | The width of the window, in unit of point. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | The width of the window, in unit of centimeter. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | The width of the window, in unit of inch. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Provides access to the workbook write protection options. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Releases resources. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Gets the default theme font name. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Set the type of print orientation for the whole workbook. |

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
