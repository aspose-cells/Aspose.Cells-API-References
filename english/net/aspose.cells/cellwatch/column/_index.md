---
title: CellWatch.Column
second_title: Aspose.Cells for .NET API Reference
description: CellWatch property. Gets and sets the column of the cell
type: docs
url: /net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Gets and sets the column of the cell.

```csharp
public int Column { get; set; }
```

### Examples

```csharp
// Called: cellWatch.Column = 1;
public static void Property_Column()
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

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


