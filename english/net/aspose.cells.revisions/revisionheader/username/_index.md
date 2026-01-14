---
title: RevisionHeader.UserName
second_title: Aspose.Cells for .NET API Reference
description: RevisionHeader property. Gets and sets the name of the user making the revision
type: docs
url: /net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Gets and sets the name of the user making the revision.

```csharp
public string UserName { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Create a RevisionHeader instance
                RevisionHeader revisionHeader = new RevisionHeader();

                // Set the UserName property
                revisionHeader.UserName = "JohnDoe";

                // Display the current value of the UserName property
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Modify the UserName property
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Save the workbook to demonstrate the property is being used
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


