---
title: Class WorkbookSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WorkbookSettings class. Represents all settings of the workbook
type: docs
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
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Gets and sets the author of the file. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Indicates whether the file is marked for auto-recovery. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Specifies the incremental public release of the application. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Indicates whether check compatibility with earlier versions when saving workbook. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Indicates whether checking custom number format when setting Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | indicates whether the application last saved the workbook file after a crash. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Gets or sets the system culture info. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | indicates whether the application last opened the workbook for data recovery. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Gets and sets default resolution of image. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Gets the settings for default values of style-related properties for this workbook. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Indicates whether discarding editting image data. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Indicates whether and how to show objects in the workbook. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Enable macros; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Gets or sets the first visible worksheet tab. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Gets the settings for formula-related features. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Gets and sets the globalization settings. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Gets and sets whether hide the field list for the PivotTable. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Gets a value that indicates whether a password is required to open this workbook. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Indicates whether this workbook is hidden. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Represents whether the generated spreadsheet will be opened Minimized. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Gets the max column index, zero-based. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Gets the max row index, zero-based. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Gets and sets the max row number of shared formula. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Gets and set the limitation of unique items per field |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Gets and sets the default print paper size. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Represents Workbook file encryption password. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Gets the protection type of the workbook. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Indicates whether setting [`QuotePrefix`](../style/quoteprefix/) property when entering the string value(which starts with single quote mark ) to the cell |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Gets or sets the regional settings for workbook. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | True if personal information can be removed from the specified workbook. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Indicates whether the application last opened the workbook in safe or repair mode. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Gets or sets a value that indicates whether the Workbook is shared. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Width of worksheet tab bar (in 1/1000 of window width). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Get or sets a value whether the Workbook tabs are displayed. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Gets and sets the number of significant digits. The default value is [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Gets the options of the smart tag. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Gets and sets the stream provider for external resource. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Indicates whether update adjacent cells' border. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Gets and sets how updates external links when the workbook is opened. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Gets or sets warning callback. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | The height of the window, in unit of point. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | The height of the window, in unit of centimeter. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | The height of the window, in unit of inch. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | The width of the window, in unit of point. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | The width of the window, in unit of centimeter. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | The width of the window, in unit of inch. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Provides access to the workbook write protection options. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Releases resources. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Gets the default theme font name. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Set the type of print orientation for the whole workbook. |

### Examples

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Create a new workbook
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Add some sample data
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Access the WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Set various settings
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Save the workbook
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


