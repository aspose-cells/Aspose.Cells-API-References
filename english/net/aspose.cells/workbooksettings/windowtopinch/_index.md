---
title: WorkbookSettings.WindowTopInch
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. The distance from the top edge of the client area to the top edge of the window in unit of inch
type: docs
url: /net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```csharp
public double WindowTopInch { get; set; }
```

### Examples

```csharp
// Called: settings.WindowTopInch = 0;
public static void Property_WindowTopInch()
    {
        // Create a new workbook
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Add some sample data
        sheet.Cells[&quot;A1&quot;].PutValue(&quot;Sample Data&quot;);
        sheet.Cells[&quot;A2&quot;].PutValue(123);
        sheet.Cells[&quot;A3&quot;].PutValue(DateTime.Now);

        // Access the WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Set various settings
        settings.Author = &quot;John Doe&quot;;
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
        settings.CultureInfo = new CultureInfo(&quot;en-US&quot;);
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = &apos;.&apos;;
        settings.NumberGroupSeparator = &apos;,&apos;;
        settings.Password = &quot;password123&quot;;
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
        settings.BuildVersion = &quot;1.0.0&quot;;
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Save the workbook
        workbook.Save(&quot;WorkbookSettingsDemo.xlsx&quot;);
    }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


