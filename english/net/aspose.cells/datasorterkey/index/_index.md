---
title: DataSorterKey.Index
second_title: Aspose.Cells for .NET API Reference
description: DataSorterKey property. Gets the sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Gets the sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Key Index: &amp;quot; + key.Index);
public static void Property_Index()
        {
            // Instantiate a new Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Score&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;John&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(85);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(90);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Doe&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(80);

            // Get the workbook&apos;s DataSorter object
            DataSorter sorter = workbook.DataSorter;

            // Set the first order for the DataSorter object
            sorter.Order1 = Aspose.Cells.SortOrder.Descending;
            // Define the first key
            sorter.Key1 = 1; // Sorting by the second column (Score)

            // Create a cells area (range)
            CellArea ca = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Sort data in the specified data range (A2:B4)
            sorter.Sort(worksheet.Cells, ca);

            // Access the DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Display the count of keys
            Console.WriteLine(&quot;Number of keys: &quot; + keys.Count);

            // Access the first key and display its properties
            DataSorterKey key = keys[0];
            Console.WriteLine(&quot;Key Index: &quot; + key.Index);
            Console.WriteLine(&quot;Key Order: &quot; + key.Order);

            // Save the workbook
            workbook.Save(&quot;DataSorterKeyCollectionExample.xlsx&quot;);
            workbook.Save(&quot;DataSorterKeyCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


