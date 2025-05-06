---
title: AutoFilter.FilterColumns
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Gets the collection of the filter columns
type: docs
url: /net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Gets the collection of the filter columns.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Examples

```csharp
// Called: FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;
public static void Property_FilterColumns()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;John&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;Doe&quot;);

            sheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(30);
            sheet.Cells[&quot;B3&quot;].PutValue(25);
            sheet.Cells[&quot;B4&quot;].PutValue(35);

            // Apply AutoFilter to the range
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Add a filter to the first column (Name)
            sheet.AutoFilter.AddFilter(0, &quot;John&quot;);

            // Add a filter to the second column (Age)
            sheet.AutoFilter.AddFilter(1, &quot;30&quot;);

            // Refresh the filter to apply it
            sheet.AutoFilter.Refresh();

            // Access the FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Access the first FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Display properties of the FilterColumn
            Console.WriteLine($&quot;IsDropdownVisible: {filterColumn.IsDropdownVisible}&quot;);
            Console.WriteLine($&quot;Filter: {filterColumn.Filter}&quot;);
            Console.WriteLine($&quot;FilterType: {filterColumn.FilterType}&quot;);
            Console.WriteLine($&quot;FieldIndex: {filterColumn.FieldIndex}&quot;);

            // Save the workbook
            workbook.Save(&quot;FilterColumnDemo.xlsx&quot;);
            workbook.Save(&quot;FilterColumnDemo.pdf&quot;);
        }
```

### See Also

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


