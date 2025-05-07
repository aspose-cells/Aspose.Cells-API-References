---
title: XmlLoadOptions.IsXmlMap
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Indicates whether mapping xml to Excel. The default value is false
type: docs
url: /net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Indicates whether mapping xml to Excel. The default value is false.

```csharp
public bool IsXmlMap { get; set; }
```

### Examples

```csharp
// Called: options.IsXmlMap = true;
public static void Property_IsXmlMap()
        {
            // Create an instance of XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Setting properties
            options.StartCell = "A1";
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = "0.00";
            options.DateFormat = "yyyy-MM-dd";
            options.IgnoreRootAttributes = false;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
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
            Workbook workbook = new Workbook("XmlLoadOptionsExample_original.xml", options);

            // Save the workbook to a new file
            workbook.Save("XmlLoadOptionsExample.xlsx");

            return;
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


