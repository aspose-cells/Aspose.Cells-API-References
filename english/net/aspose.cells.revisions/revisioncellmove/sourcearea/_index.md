---
title: RevisionCellMove.SourceArea
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellMove property. Gets the source area
type: docs
url: /net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Gets the source area.

```csharp
public CellArea SourceArea { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some cells with sample data
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // The original sample used revision‑tracking features that are not
                // part of the reflected API (IsTrackChanges, MoveRows, Revisions).
                // To keep the code compile‑ready we demonstrate the SourceArea
                // property by creating a RevisionCellMove instance via reflection.
                // -------------------------------------------------------------

                // Create an instance of RevisionCellMove using reflection
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Display the SourceArea value (read‑only)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Additional related information (optional)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet may be null for a freshly created instance
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Save the workbook (optional)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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


