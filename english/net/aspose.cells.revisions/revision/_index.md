---
title: Class Revision
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.Revision class. Represents the revision
type: docs
url: /net/aspose.cells.revisions/revision/
---
## Revision class

Represents the revision.

```csharp
public abstract class Revision
```

## Properties

| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add some data to potentially create revisions
                worksheet.Cells["A1"].PutValue("Original Value");

                // Save the workbook to establish a baseline
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Load the workbook and make a change
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Check if there are any revision logs
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Get the first revision
                        Revision revision = log.Revisions[0];

                        // Display read-only properties
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Save the modified workbook
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


