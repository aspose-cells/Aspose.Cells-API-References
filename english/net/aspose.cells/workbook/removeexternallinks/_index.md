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
namespace AsposeCellsExamples.WorkbookMethodRemoveExternalLinksDemo
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some external links for demonstration
            worksheet.Cells["A1"].Formula = "=SUM([ExternalWorkbook.xlsx]Sheet1!A1:A10)";
            worksheet.Cells["A2"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!B1";

            Console.WriteLine("Workbook contains external links before removal: " + 
                (workbook.HasExernalLinks() ? "Yes" : "No"));

            try
            {
                // Call the RemoveExternalLinks method
                workbook.RemoveExternalLinks();
                
                Console.WriteLine("Method executed successfully");
                Console.WriteLine("Workbook contains external links after removal: " + 
                    (workbook.HasExernalLinks() ? "Yes" : "No"));

                // Show the effect on the formulas
                Console.WriteLine("Cell A1 formula after removal: " + worksheet.Cells["A1"].Formula);
                Console.WriteLine("Cell A2 formula after removal: " + worksheet.Cells["A2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveExternalLinks method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("MethodRemoveExternalLinksDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


