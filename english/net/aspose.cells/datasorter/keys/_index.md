---
title: DataSorter.Keys
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Gets the key list of data sorter
type: docs
url: /net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Gets the key list of data sorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Examples

```csharp
// Called: DataSorterKeyCollection keys = sorter.Keys;
public static void Property_Keys()
        {
            // Create a workbook object and load a template file
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to sort
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;USA&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;China&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Brazil&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Russia&quot;);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Canada&quot;);

            // Instantiate data sorter object
            DataSorter sorter = workbook.DataSorter;

            // Add key for the first column (A) to sort in ascending order
            sorter.AddKey(0, SortOrder.Ascending);

            // Create a cell area (range) to sort
            CellArea ca = CellArea.CreateCellArea(&quot;A1&quot;, &quot;A5&quot;);

            // Perform the sort
            sorter.Sort(worksheet.Cells, ca);

            // Save the output file
            workbook.Save(&quot;DataSorterKeyExample.xlsx&quot;);
            workbook.Save(&quot;DataSorterKeyExample.pdf&quot;);

            // Access the DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Iterate through the keys and print their properties
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($&quot;Order: {key.Order}&quot;);
                Console.WriteLine($&quot;Index: {key.Index}&quot;);
                Console.WriteLine($&quot;Type: {key.Type}&quot;);
                Console.WriteLine($&quot;IconSetType: {key.IconSetType}&quot;);
                Console.WriteLine($&quot;IconId: {key.IconId}&quot;);
                Console.WriteLine($&quot;Color: {key.Color}&quot;);
            }
        }
```

### See Also

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


