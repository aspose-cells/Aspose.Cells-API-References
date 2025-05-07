---
title: DataSorterKeyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: DataSorterKeyCollection property. Gets and sets DataSorterKey by index
type: docs
url: /net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Gets and sets [`DataSorterKey`](../../datasorterkey/) by index.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: DataSorterKey key = keys[0];
public static void Property_Int32_()
        {
            // Instantiate a new Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            // Get the workbook's DataSorter object
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
            Console.WriteLine("Number of keys: " + keys.Count);

            // Access the first key and display its properties
            DataSorterKey key = keys[0];
            Console.WriteLine("Key Index: " + key.Index);
            Console.WriteLine("Key Order: " + key.Order);

            // Save the workbook
            workbook.Save("DataSorterKeyCollectionExample.xlsx");
            workbook.Save("DataSorterKeyCollectionExample.pdf");
            return;
        }
```

### See Also

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


