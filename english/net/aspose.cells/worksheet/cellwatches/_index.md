---
title: Worksheet.CellWatches
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets collection of cells on this worksheet being watched in the watch window
type: docs
url: /net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Gets collection of cells on this worksheet being watched in the 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Examples

```csharp
// Called: int watchIndex = sheet.CellWatches.Add("B2");
public static void Worksheet_Property_CellWatches()
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

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


