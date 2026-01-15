---
title: Workbook.RemoveExternalLinks
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes all external links in the workbook
type: docs
url: /net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Removes all external links in the workbook.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Clear() method. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Call the RemoveExternalLinks method
                workbook.RemoveExternalLinks();

                // Display results or effects of the method call
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Save the workbook if changes were made
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


