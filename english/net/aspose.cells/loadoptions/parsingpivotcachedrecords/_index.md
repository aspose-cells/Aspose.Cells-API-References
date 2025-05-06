---
title: LoadOptions.ParsingPivotCachedRecords
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether parsing pivot cached records when loading the file. The default value is false
type: docs
url: /net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Indicates whether parsing pivot cached records when loading the file. The default value is false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Remarks

Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### Examples

```csharp
// Called: loadOptions.ParsingPivotCachedRecords = false;
public static void Property_ParsingPivotCachedRecords()
        {
            // Create an instance of LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Setting properties
            loadOptions.Password = &quot;password123&quot;;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo(&quot;en-US&quot;);
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
            Workbook workbook = new Workbook(&quot;LoadOptionsExample_original.xlsx&quot;, loadOptions);

            // Perform operations on the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello, World!&quot;);

            // Save the workbook
            workbook.Save(&quot;LoadOptionsExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


