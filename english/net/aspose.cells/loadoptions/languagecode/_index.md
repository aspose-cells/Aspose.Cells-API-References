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
// Called: loadOptions.LanguageCode = CountryCode.USA;
public static void LoadOptions_Property_LanguageCode()
        {
            // Create an instance of LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Setting properties
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Load a workbook with the specified LoadOptions
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Perform operations on the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Save the workbook
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


