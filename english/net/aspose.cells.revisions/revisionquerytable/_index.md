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
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to create a context for query table
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Note: RevisionQueryTable instances are typically obtained from workbook revisions
                // This is a conceptual demonstration since we can't directly instantiate RevisionQueryTable

                // In a real scenario, you would access revisions like this:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Access properties
                //     }
                // }

                // For demonstration, we'll show how to work with RevisionQueryTable properties
                // if we had an instance
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Save the workbook
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


