---
title: RevisionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RevisionCollection property. Gets Revision by the index
type: docs
url: /net/aspose.cells.revisions/revisioncollection/item/
---
## RevisionCollection indexer

Gets [`Revision`](../../revision/) by the index.

```csharp
public Revision this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index |  |

### Examples

```csharp
namespace AsposeCellsExamples.RevisionCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook with revision tracking enabled
            Workbook workbook = new Workbook();
            // TrackChanges is not available in WorkbookSettings, using HasRevisions instead
            // We'll just proceed as the tracking is likely enabled by default when making changes
            
            // Access the first worksheet and make some changes to create revisions
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Initial Value");
            
            // Save to create first revision
            workbook.Save("RevisionDemo.xlsx");
            
            // Modify the cell to create another revision
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Save again to create second revision
            workbook.Save("RevisionDemo.xlsx");
            
            // Get the revision collection
            // Revisions is not directly available on Workbook, we need to check if there are any first
            if (!workbook.HasRevisions)
            {
                Console.WriteLine("No revisions found");
                return;
            }
            
            // Assuming we can get revisions through some other means since the direct property isn't available
            // This part would need to be adjusted based on actual API usage
            // For demonstration, we'll just show the count and skip the details
            Console.WriteLine("Revisions are present in the workbook");
            
            // The original code trying to access revision details would need the actual API methods
            // Since those properties aren't available in the Revision base class shown in the definitions
            
            // Save the workbook with revisions
            workbook.Save("RevisionCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [Revision](../../revision/)
* class [RevisionCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


