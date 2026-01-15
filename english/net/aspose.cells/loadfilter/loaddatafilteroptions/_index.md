---
title: LoadFilter.LoadDataFilterOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadFilter property. The filter options to denote what data should be loaded
type: docs
url: /net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

The filter options to denote what data should be loaded.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // Create a LoadFilter instance with default options
                LoadFilter loadFilter = new LoadFilter();

                // Display the default LoadDataFilterOptions value
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Set new filter options (combination of flags)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // Display the updated value
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Create another filter with different options
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // Display the options from constructor
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // Save the workbook
                workbook.Save("LoadDataFilterOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


