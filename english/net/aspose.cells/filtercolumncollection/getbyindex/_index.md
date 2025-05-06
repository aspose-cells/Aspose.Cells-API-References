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
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to filter
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;John&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(25);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(30);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Doe&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(22);

            // Create an AutoFilter
            worksheet.AutoFilter.Range = &quot;A1:B4&quot;;

            // Get the FilterColumnCollection
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // Add a filter to the second column (Age)
            worksheet.AutoFilter.AddFilter(1, &quot;25&quot;);

            // Apply the filter
            worksheet.AutoFilter.Refresh();

            // Access and manipulate the FilterColumnCollection
            Console.WriteLine(&quot;Number of filters applied: &quot; + filterColumns.Count);

            // Get the first filter column
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine(&quot;Filter applied on column index: &quot; + filterColumn.FieldIndex);

            // Remove the filter
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // Save the workbook
            workbook.Save(&quot;FilterColumnCollectionExample.xlsx&quot;);
            workbook.Save(&quot;FilterColumnCollectionExample.pdf&quot;);
        }
```

### See Also

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


