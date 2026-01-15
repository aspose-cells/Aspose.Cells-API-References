---
title: Class RevisionRenameSheet
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionRenameSheet class. Represents a revision of renaming sheet
type: docs
url: /net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Represents a revision of renaming sheet.

```csharp
public class RevisionRenameSheet : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Gets the new name of the worksheet. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Gets the old name of the worksheet. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Represents the type of the revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Store original name and rename the sheet
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Save to memory stream to generate revisions
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Reopen the workbook to access revision logs
                workbook = new Workbook(ms);

                // Check revision logs for rename operation
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


