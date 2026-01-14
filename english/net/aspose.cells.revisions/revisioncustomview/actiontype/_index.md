---
title: RevisionCustomView.ActionType
second_title: Aspose.Cells for .NET API Reference
description: RevisionCustomView property. Gets the type of action
type: docs
url: /net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Gets the type of action.

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

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Load an existing workbook that might contain custom view revisions
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Iterate through all revision logs in the workbook
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Check each revision in the log
                    foreach (Revision revision in log.Revisions)
                    {
                        // Check if this is a custom view revision
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Display the ActionType property value
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Demonstrate how to use the ActionType property
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Display additional properties for context
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
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
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


