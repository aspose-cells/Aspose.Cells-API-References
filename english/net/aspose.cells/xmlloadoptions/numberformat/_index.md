---
title: XmlLoadOptions.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Gets and sets the format of numeric value
type: docs
url: /net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Gets and sets the format of numeric value.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: options.NumberFormat = &amp;quot;0.00&amp;quot;;
public static void Property_NumberFormat()
        {
            // Create an instance of XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Setting properties
            options.StartCell = &quot;A1&quot;;
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = &quot;0.00&quot;;
            options.DateFormat = &quot;yyyy-MM-dd&quot;;
            options.IgnoreRootAttributes = false;
            options.Password = &quot;password&quot;;
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo(&quot;en-US&quot;);
            options.StandardFont = &quot;Arial&quot;;
            options.StandardFontSize = 10.5;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            options.LightCellsDataHandler = null; // Assuming no data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = null; // Assuming no individual font configs are set
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = false;

            // Load an XML file into a Workbook using the specified options
            Workbook workbook = new Workbook(&quot;XmlLoadOptionsExample_original.xml&quot;, options);

            // Save the workbook to a new file
            workbook.Save(&quot;XmlLoadOptionsExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


