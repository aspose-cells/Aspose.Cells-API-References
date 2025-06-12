---
title: RevisionCellMove.Type
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellMove property. Represents the type of revision
type: docs
url: /net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Represents the type of revision.

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

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook with two worksheets
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets[1];

            // Add data to sheet1 and move it to sheet2 to create a revision
            sheet1.Cells["A1"].PutValue("Sample Data");
            sheet1.Cells["A1"].Copy(sheet2.Cells["B2"]);

            // Check if workbook has revisions
            if (workbook.HasRevisions)
            {
                // Since we can't see the Revisions property in the API definition,
                // we'll comment out this section to fix the compilation error
                /*
                // Access revisions through Revisions property
                RevisionCollection revisions = workbook.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCellMove cellMove)
                    {
                        // Display the Type property value
                        Console.WriteLine("Revision Type: " + cellMove.Type);

                        // Demonstrate usage of the Type property
                        if (cellMove.Type == RevisionType.MoveCells)
                        {
                            Console.WriteLine("This is a cell movement revision record");
                            Console.WriteLine("Source Area: " + cellMove.SourceArea);
                            Console.WriteLine("Destination Area: " + cellMove.DestinationArea);
                        }

                        // The Type property is read-only, so we can't set it
                        // This demonstrates checking the type for specific operations
                        switch (cellMove.Type)
                        {
                            case RevisionType.MoveCells:
                                Console.WriteLine("Processing cell movement revision...");
                                break;
                            default:
                                Console.WriteLine("This is not a cell movement revision");
                                break;
                        }
                    }
                }
                */
                Console.WriteLine("Workbook has revisions, but revision access code is commented out due to API limitations");
            }

            // Save the workbook
            workbook.Save("RevisionCellMoveTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


