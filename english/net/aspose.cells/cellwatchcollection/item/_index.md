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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Demonstrate Item property usage
            CellWatch cellWatch = cellWatches[watchIndex];
            
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A1";
            
            Console.WriteLine("\nModified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            workbook.Save("CellWatchCollectionExample.xlsx");
        }
    }
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a cell watch to the collection
                int watchIndex = worksheet.CellWatches.Add("A1");

                // Access the CellWatchCollection
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // Demonstrate accessing the Item property using indexer
                CellWatch cellWatch = cellWatches[watchIndex];

                // Display the properties of the CellWatch item
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Save the workbook
                workbook.Save("CellWatchItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated successfully.");
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

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


