---
title: RevisionInsertDelete.ActionType
second_title: Aspose.Cells for .NET API Reference
description: RevisionInsertDelete property. Gets the action type of this revision
type: docs
url: /net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Gets the action type of this revision.

```csharp
public RevisionActionType ActionType { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook and enable revision tracking
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Perform operations to generate insert/delete revisions
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Get the revision logs
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Iterate through all revision logs to find insert/delete revisions
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Display the ActionType property value
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Demonstrate different action types
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Show related information
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Save the workbook with revisions
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


