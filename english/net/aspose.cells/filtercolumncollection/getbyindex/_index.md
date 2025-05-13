---
title: FilterColumnCollection.GetByIndex
second_title: Aspose.Cells for .NET API Reference
description: FilterColumnCollection method. Returns a single Filter object from a collection
type: docs
url: /net/aspose.cells/filtercolumncollection/getbyindex/
---
## FilterColumnCollection.GetByIndex method

Returns a single Filter object from a collection.

```csharp
public FilterColumn GetByIndex(int index)
```

### Examples

```csharp
// Called: FilterColumn filterColumn = filterColumns.GetByIndex(0);
public static void FilterColumnCollection_Method_GetByIndex()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to filter
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);

            // Create an AutoFilter
            worksheet.AutoFilter.Range = "A1:B4";

            // Get the FilterColumnCollection
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // Add a filter to the second column (Age)
            worksheet.AutoFilter.AddFilter(1, "25");

            // Apply the filter
            worksheet.AutoFilter.Refresh();

            // Access and manipulate the FilterColumnCollection
            Console.WriteLine("Number of filters applied: " + filterColumns.Count);

            // Get the first filter column
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter applied on column index: " + filterColumn.FieldIndex);

            // Remove the filter
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // Save the workbook
            workbook.Save("FilterColumnCollectionExample.xlsx");
            workbook.Save("FilterColumnCollectionExample.pdf");
        }
```

### See Also

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


