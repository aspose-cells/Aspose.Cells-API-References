---
title: Class RevisionCustomView
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionCustomView class. Represents a revision record of adding or removing a custom view to the workbook
type: docs
url: /net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Represents a revision record of adding or removing a custom view to the workbook

```csharp
public class RevisionCustomView : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | Gets the type of action. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Gets the globally unique identifier of the custom view. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Gets the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCustomViewDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add a custom view to potentially generate a revision
                // Note: Using CustomDocumentProperties as a workaround since CustomViews isn't available
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Access the revision logs (assuming they exist)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Display the read-only properties
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Demonstrate basic usage of the properties
                            if (customViewRevision.Type == RevisionType.CustomView)
                            {
                                Console.WriteLine("This is a custom view revision.");
                            }

                            if (customViewRevision.ActionType == RevisionActionType.Add)
                            {
                                Console.WriteLine("The custom view was added.");
                            }
                            else if (customViewRevision.ActionType == RevisionActionType.Delete)
                            {
                                Console.WriteLine("The custom view was deleted.");
                            }
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionCustomViewDemo.xlsx");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


