---
title: CellWatchCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CellWatchCollection property. Gets and sets CellWatch by index
type: docs
url: /net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Gets and sets [`CellWatch`](../../cellwatch/) by index.

```csharp
public CellWatch this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: CellWatch cellWatch = cellWatches[watchIndex];
public static void CellWatchCollection_Property_Item()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Get the first Worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add Cell Watch Item into the watch window
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // Access the CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Access the added CellWatch item
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Display the properties of the CellWatch item
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Modify the properties of the CellWatch item
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // Display the modified properties of the CellWatch item
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Save the workbook
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
```

### See Also

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Gets and sets [`CellWatch`](../../cellwatch/) by the name of the cell.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | The name of the cell. |

### Examples

```csharp
namespace AsposeCellsExamples.CellWatchCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the CellWatchCollection
            CellWatchCollection watchCollection = worksheet.CellWatches;

            // Add cells to watch
            int index1 = watchCollection.Add("A1");
            int index2 = watchCollection.Add(1, 0); // B2

            // Access items using the Item property
            CellWatch watch1 = watchCollection[index1];
            CellWatch watch2 = watchCollection[index2];

            // Display information about watched cells
            Console.WriteLine("Watched Cell 1: " + watch1.CellName);
            Console.WriteLine("Watched Cell 2: " + watch2.CellName);

            // Modify cell values to demonstrate watching functionality
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B2"].PutValue(123.45);

            // Save the workbook
            workbook.Save("CellWatchCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


