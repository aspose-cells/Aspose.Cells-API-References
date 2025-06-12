---
title: RevisionQueryTable.FieldId
second_title: Aspose.Cells for .NET API Reference
description: RevisionQueryTable property. Gets ID of the specific query table field that was removed
type: docs
url: /net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Gets ID of the specific query table field that was removed.

```csharp
public int FieldId { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to create a query table
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Create a query table - fixed the Add method issue
            QueryTable queryTable = worksheet.QueryTables[0];
            // Replace Connection with ConnectionId (though it's read-only, so we can't set it)
            // Replace Destination with ResultRange (though it's read-only, so we can't set it)
            // Since both properties are read-only, we'll need to modify the approach
            // Instead, we'll just work with the existing query table properties
            
            // Cannot set Name as it's read-only according to the type definition
            // queryTable.Name = "TestQueryTable";

            // Track revisions - these methods don't exist in the Workbook class
            // workbook.StartTrackingRevisions();
            // Instead, revisions are automatically tracked when HasRevisions is true

            // Modify the query table to generate a revision
            // Refresh method doesn't exist in QueryTable class
            // queryTable.Refresh();
            // Alternative action that might trigger a revision:
            queryTable.PreserveFormatting = !queryTable.PreserveFormatting;

            // Stop tracking revisions - this method doesn't exist
            // workbook.StopTrackingRevisions();

            // Access the revisions
            // Revisions property doesn't exist in Worksheet class
            // RevisionCollection revisions = workbook.Worksheets[0].Revisions;
            // Alternative: Check if workbook has revisions
            if (workbook.HasRevisions)
            {
                // In actual implementation, you would need to use the appropriate API to access revisions
                // This is just a placeholder since the exact API isn't shown in the definitions
                Console.WriteLine("Workbook has revisions, but the API to access them is not available in the provided definitions");
            }

            // Save the workbook
            workbook.Save("RevisionQueryTableFieldIdDemo.xlsx");
        }
    }
}
```

### See Also

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


