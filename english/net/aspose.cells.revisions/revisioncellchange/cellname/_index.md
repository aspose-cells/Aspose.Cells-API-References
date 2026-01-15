---
title: RevisionCellChange.CellName
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellChange property. Gets the name of the cell
type: docs
url: /net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

Gets the name of the cell.

```csharp
public string CellName { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyCellNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add initial data to create a revision
            worksheet.Cells["A1"].PutValue("Original Value");

            // Modify the cell to create a revision
            worksheet.Cells["A1"].PutValue("Modified Value");

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
                            // Display the CellName property value
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);

                            // Demonstrate using the CellName property
                            if (cellChange.CellName == "A1")
                            {
                                Console.WriteLine("\nThe revision is for cell A1");
                                Console.WriteLine("Old Value: " + cellChange.OldValue);
                                Console.WriteLine("New Value: " + cellChange.NewValue);
                            }
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionCellChangePropertyCellNameDemo.xlsx");
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


