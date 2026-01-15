---
title: PivotTable.PivotFilters
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns all filters of pivot fields in the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Returns all filters of pivot fields in the pivot table.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Create a pivot table
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Add fields to the pivot table
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Access the PivotFilters collection (read-only property)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Display information about the PivotFilters collection
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Iterate through the filters and display their types
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Add a sample filter to demonstrate functionality
                if (pivotFilters.Count == 0)
                {
                    // Add a value filter to the first field (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Display updated filter count
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Save the workbook
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
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

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


