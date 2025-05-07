---
title: CellWatch.Row
second_title: Aspose.Cells for .NET API Reference
description: CellWatch property. Gets and sets the row of the cell
type: docs
url: /net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Gets and sets the row of the cell.

```csharp
public int Row { get; set; }
```

### Examples

```csharp
// Called: cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
public static void Property_Row()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Get the first Worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Add Cell Watch Item into the watch window
            int watchIndex = sheet.CellWatches.Add("B2");

            // Retrieve the CellWatch object
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Setting properties
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Save the workbook
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
```

### See Also

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


