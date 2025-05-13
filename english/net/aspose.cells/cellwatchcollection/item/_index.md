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

### See Also

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


