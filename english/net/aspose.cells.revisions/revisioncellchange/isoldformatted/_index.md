---
title: RevisionCellChange.IsOldFormatted
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellChange property. Indicates whether this cell is old formatted
type: docs
url: /net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

Indicates whether this cell is old formatted.

```csharp
public bool IsOldFormatted { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set initial cell value and style
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // Change the cell value and style to create a revision
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

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
                            // Display the IsOldFormatted property value
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);

                            // Show additional context about the revision
                            if (cellChange.IsOldFormatted)
                            {
                                Console.WriteLine("The cell had formatting before this revision.");
                                Console.WriteLine("Old Font: " + cellChange.OldStyle.Font.Name);
                                Console.WriteLine("Old Font Size: " + cellChange.OldStyle.Font.Size);
                            }
                            else
                            {
                                Console.WriteLine("The cell did not have formatting before this revision.");
                            }
                        }
                    }
                }

                // Save the workbook with revisions
                workbook.Save("IsOldFormattedDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved as IsOldFormattedDemo.xlsx");
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


