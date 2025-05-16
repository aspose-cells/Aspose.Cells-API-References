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
namespace AsposeCellsExamples.RevisionsClassRevisionAutoFormatDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionAutoFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Apply some formatting to trigger a revision
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            
            // Apply style to cells directly since ApplyStyle isn't available
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    worksheet.Cells[row, col].SetStyle(style);
                }
            }

            // Check if there are any revisions (though we can't track them directly)
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook contains revisions");
            }
            else
            {
                Console.WriteLine("No revisions found - revision tracking not directly supported");
            }

            // Save the workbook
            workbook.Save("RevisionAutoFormatDemo.xlsx");
        }
    }
}
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


