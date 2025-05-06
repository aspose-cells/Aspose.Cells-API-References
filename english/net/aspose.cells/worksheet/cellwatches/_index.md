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
// Called: CellWatch cellWatch = sheet.CellWatches[watchIndex];
public static void Property_CellWatches()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Get the first Worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Add Cell Watch Item into the watch window
            int watchIndex = sheet.CellWatches.Add(&quot;B2&quot;);

            // Retrieve the CellWatch object
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Setting properties
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = &quot;B2&quot;;

            // Save the workbook
            workbook.Save(&quot;CellWatchExample.xlsx&quot;);
            workbook.Save(&quot;CellWatchExample.pdf&quot;);
            return;
        }
```

### See Also

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


