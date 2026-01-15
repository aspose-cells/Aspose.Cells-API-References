---
title: RevisionCellMove.DestinationArea
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellMove property. Gets the destination area
type: docs
url: /net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Gets the destination area.

```csharp
public CellArea DestinationArea { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // Create a workbook to have a valid environment (optional for the demo)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Instantiate RevisionCellMove via reflection (parameterless ctor)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // Read and display the DestinationArea property (read‑only)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Additional context (optional)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Save workbook (optional)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


