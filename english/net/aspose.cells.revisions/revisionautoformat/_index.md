---
title: Class RevisionAutoFormat
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionAutoFormat class. represents a revision record of information about a formatting change
type: docs
url: /net/aspose.cells.revisions/revisionautoformat/
---
## RevisionAutoFormat class

represents a revision record of information about a formatting change.

```csharp
public class RevisionAutoFormat : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionautoformat/cellarea/) { get; } | Gets the location where the formatting was applied. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionautoformat/type/) { get; } | Gets the type of the revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionAutoFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();

            try
            {
                // Access the revision logs collection
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Find the first RevisionAutoFormat instance
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Demonstrate the Type property (read-only)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");

                    // Demonstrate the CellArea property (read-only)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionAutoFormat: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


