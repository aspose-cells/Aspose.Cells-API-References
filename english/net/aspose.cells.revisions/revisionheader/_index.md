---
title: Class RevisionHeader
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionHeader class. Represents a list of specific changes that have taken place for this workbook
type: docs
url: /net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Represents a list of specific changes that have taken place for this workbook.

```csharp
public class RevisionHeader
```

## Constructors

| Name | Description |
| --- | --- |
| [RevisionHeader](revisionheader/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Gets and sets rhe date and time when this set of revisions was saved. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Gets and sets the name of the user making the revision. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create an instance of the RevisionHeader class
                RevisionHeader revisionHeader = new RevisionHeader();

                // Set essential properties
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Demonstrate basic functionality
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Save the workbook
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


