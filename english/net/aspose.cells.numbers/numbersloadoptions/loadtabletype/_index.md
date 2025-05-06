---
title: NumbersLoadOptions.LoadTableType
second_title: Aspose.Cells for .NET API Reference
description: NumbersLoadOptions property. Gets and sets the type of loading multiple tables in one worksheet
type: docs
url: /net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Gets and sets the type of loading multiple tables in one worksheet.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Examples

```csharp
// Called: LoadTableType = LoadNumbersTableType.OneTablePerSheet,
public static void Property_LoadTableType()
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

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


