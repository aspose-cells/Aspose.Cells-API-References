---
title: RevisionInsertSheet.Name
second_title: Aspose.Cells for .NET API Reference
description: RevisionInsertSheet property. Gets the name of the worksheet
type: docs
url: /net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Gets the name of the worksheet.

```csharp
public string Name { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to potentially generate a revision record
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simulate accessing a RevisionInsertSheet from revisions
                // Note: In a real scenario, this would come from workbook.Revisions
                // For demonstration, we'll create a mock scenario
                RevisionInsertSheet insertSheetRevision = null;

                // In actual usage, you would get this from the revisions collection
                // For example: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Since we can't create RevisionInsertSheet directly, we'll demonstrate
                // what you would do if you had access to one
                if (insertSheetRevision != null)
                {
                    // Display the Name property value (read-only)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Demonstrate using the Name property in a conditional check
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Save the workbook
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


