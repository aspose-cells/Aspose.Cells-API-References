---
title: LoadOptions.LanguageCode
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file
type: docs
url: /net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Examples

```csharp
// Called: LanguageCode = CountryCode.USA,
public static void Property_LanguageCode()
        {
            // Create an instance of NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Setting properties
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                Password = &quot;password123&quot;,
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = false,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new CultureInfo(&quot;en-US&quot;),
                StandardFont = &quot;Arial&quot;,
                StandardFontSize = 10.5,
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new CustomLightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new CustomWarningCallback(),
                AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true },
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = false
            };

            // Load a Numbers file with the specified load options
            Workbook workbook = new Workbook(&quot;NumbersLoadOptionsExample_original.numbers&quot;, loadOptions);

            // Save the workbook in XLSX format
            workbook.Save(&quot;NumbersLoadOptionsExample.xlsx&quot;);
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


