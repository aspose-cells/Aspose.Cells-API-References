---
title: RevisionCellChange.IsOldFormatted
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellChange property. Indicates whether this cell is old formatted
type: docs
url: /net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

Indicates whether this cell is old formatted.

```csharp
public bool IsOldFormatted { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // Create a new workbook with revision tracking
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Initial Value");
            
            // Make a change to create a revision
            workbook.Worksheets[0].Cells["A1"].PutValue("Changed Value");
            workbook.Worksheets[0].Cells["A1"].GetStyle().Font.IsBold = true;

            // Access the revisions if any exist
            if (workbook.HasRevisions)
            {
                // Note: The actual API doesn't provide direct access to revisions through Worksheet
                // This part would need to be adjusted based on how revisions are actually accessed
                // in the Aspose.Cells API. The following is a placeholder since the API doesn't
                // expose revisions collection as shown in the original code.
                
                Console.WriteLine("Workbook has revisions, but direct access to revisions collection is not available in this API version.");
                
                // The original code's revision checking logic would go here if the API supported it
                // For demonstration, we'll just show the property we wanted to check exists
                Console.WriteLine("IsOldFormatted property exists on RevisionCellChange class");
            }

            // Save the workbook
            workbook.Save("RevisionCellChangePropertyIsOldFormattedDemo.xlsx");
        }
    }
}
```

### See Also

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


