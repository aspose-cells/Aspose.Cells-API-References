---
title: RevisionCustomView.Guid
second_title: Aspose.Cells for .NET API Reference
description: RevisionCustomView property. Gets the globally unique identifier of the custom view
type: docs
url: /net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Gets the globally unique identifier of the custom view.

```csharp
public Guid Guid { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // Open an existing workbook that contains custom view revisions
            Workbook workbook = new Workbook("example.xlsx");
            
            // Process revision logs
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### See Also

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


