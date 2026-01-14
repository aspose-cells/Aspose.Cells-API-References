---
title: RevisionLogCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RevisionLogCollection property. Gets RevisionLog by index
type: docs
url: /net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Gets [`RevisionLog`](../../revisionlog/) by index.

```csharp
public RevisionLog this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

Returns [`RevisionLog`](../../revisionlog/) object.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Enable shared workbook to support revisions
            workbook.Settings.Shared = true;

            // Access the revision logs collection
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Check if there are any revision logs
                if (revisionLogs.Count > 0)
                {
                    // Access the first revision log using the Item property
                    RevisionLog firstLog = revisionLogs[0];

                    // Display basic information about the revision log
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Save the workbook
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


