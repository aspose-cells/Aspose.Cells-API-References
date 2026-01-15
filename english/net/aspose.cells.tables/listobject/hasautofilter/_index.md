---
title: ListObject.HasAutoFilter
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether auto filter is applied to this table
type: docs
url: /net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Indicates whether auto filter is applied to this table.

```csharp
public bool HasAutoFilter { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data for the table
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Add a ListObject (table) covering the data range
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Ensure the table is resized to include all rows
                listObject.Resize(0, 0, 4, 2, true);

                // Read and display the HasAutoFilter property value
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // The AutoFilter object can be accessed via the AutoFilter property
                // Demonstrate that it is not null when HasAutoFilter is true
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Apply a simple filter on the "Score" column (index 1) to show rows with Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Use Cells.Rows to check if the row is hidden
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Clear the filter
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Save the workbook (optional)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


