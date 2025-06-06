---
title: DataSorterKey.IconSetType
second_title: Aspose.Cells for .NET API Reference
description: DataSorterKey property. Represents the icon set type
type: docs
url: /net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Represents the icon set type.

```csharp
public IconSetType IconSetType { get; }
```

### Remarks

Only takes effect when [`Type`](../type/) is Icon.

### Examples

```csharp
// Called: Console.WriteLine($"IconSetType: {key.IconSetType}");
public static void DataSorterKey_Property_IconSetType()
        {
            // Create a workbook object and load a template file
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to sort
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Instantiate data sorter object
            DataSorter sorter = workbook.DataSorter;

            // Add key for the first column (A) to sort in ascending order
            sorter.AddKey(0, SortOrder.Ascending);

            // Create a cell area (range) to sort
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Perform the sort
            sorter.Sort(worksheet.Cells, ca);

            // Save the output file
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Access the DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Iterate through the keys and print their properties
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


