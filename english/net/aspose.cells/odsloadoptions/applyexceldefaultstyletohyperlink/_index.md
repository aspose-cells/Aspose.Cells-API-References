---
title: OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink
second_title: Aspose.Cells for .NET API Reference
description: OdsLoadOptions property. Indicates whether applying the default style of the Excel to hyperlink
type: docs
url: /net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Indicates whether applying the default style of the Excel to hyperlink.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Examples

```csharp
// Called: loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
public static void OdsLoadOptions_Property_ApplyExcelDefaultStyleToHyperlink()
        {
            // Create an instance of OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Setting properties
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            loadOptions.RefreshPivotTables = true;
            loadOptions.Password = "your_password";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new System.Globalization.CultureInfo("en-US");
            loadOptions.StandardFont = "Arial";
            loadOptions.StandardFontSize = 10.5;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.WarningCallback = new CustomWarningCallback();
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.FontConfigs = new IndividualFontConfigs();
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Load an ODS file with the specified options
            Workbook workbook = new Workbook("OdsLoadOptionsExample_original.ods", loadOptions);

            // Save the workbook to a new file
            workbook.Save("OdsLoadOptionsExample.xlsx");

            return;
        }
```

### See Also

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


