---
title: RevisionFormat.Type
second_title: Aspose.Cells for .NET API Reference
description: RevisionFormat property. Gets the type of revision
type: docs
url: /net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Gets the type of revision.

```csharp
public override RevisionType Type { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Note: Aspose.Cells doesn't have StartTrackRevisions method in the Workbook class
            // Tracking revisions is automatically handled when changes are made to a shared workbook
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Make some formatting changes to track revisions
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            cell.SetStyle(style);

            // Note: Aspose.Cells doesn't have Revisions property in the Workbook class
            // We can only check if there are revisions using HasRevisions property
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook contains revisions");
                // Unfortunately we can't access the revisions collection directly
            }

            // Save the workbook with revisions
            workbook.Save("RevisionFormatPropertyTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


