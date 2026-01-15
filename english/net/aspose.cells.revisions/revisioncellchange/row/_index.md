---
title: RevisionCellChange.Row
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellChange property. Gets the row index of the cell
type: docs
url: /net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

Gets the row index of the cell.

```csharp
public int Row { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add initial data to create a revision
            worksheet.Cells["B5"].PutValue("Original Value");

            // Modify the cell to create a revision
            worksheet.Cells["B5"].PutValue("Modified Value");

            try
            {
                // Access the revision logs
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Display the Row property value
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demonstrate using the Row property
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


