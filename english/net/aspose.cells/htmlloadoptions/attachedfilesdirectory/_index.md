---
title: HtmlLoadOptions.AttachedFilesDirectory
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. The directory that the attached files will be saved to
type: docs
url: /net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

The directory that the attached files will be saved to.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: options.AttachedFilesDirectory = "C:\\AttachedFiles";
public static void Property_AttachedFilesDirectory()
        {
            // Create an instance of EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // Setting properties
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // Load an ebook file into a Workbook using the specified options
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // Save the workbook to an Excel file
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


