---
title: Class RevisionQueryTable
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionQueryTable class. Represents a revision of a query table field change
type: docs
url: /net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Represents a revision of a query table field change.

```csharp
public class RevisionQueryTable : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Gets the location of the affected query table. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Gets ID of the specific query table field that was removed. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Represents the type of the revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Since we can't directly create a RevisionQueryTable instance (no public constructor shown),
                // we'll demonstrate accessing properties from an existing revision
                if (workbook.HasRevisions)
                {
                    // Note: In real usage, you would get revisions from the workbook's revision collection
                    // This is just a demonstration of property access
                    Console.WriteLine("Workbook has revisions");
                    
                    // Example of how you might work with a RevisionQueryTable if you had one
                    // RevisionQueryTable revision = GetExistingRevisionQueryTable(workbook);
                    // Console.WriteLine($"Revision Type: {revision.Type}");
                    // Console.WriteLine($"Cell Area: {revision.CellArea}");
                    // Console.WriteLine($"Field ID: {revision.FieldId}");
                }
                else
                {
                    Console.WriteLine("No revisions found in workbook");
                }

                // Save the workbook
                workbook.Save("RevisionsClassRevisionQueryTableDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


