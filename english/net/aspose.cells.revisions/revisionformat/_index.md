---
title: Class RevisionFormat
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionFormat class. Represents a revision record of information about a formatting change
type: docs
url: /net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Represents a revision record of information about a formatting change.

```csharp
public class RevisionFormat : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | The range to which this formatting was applied. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Gets the applied style. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Gets the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook with shared mode to enable revision tracking
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add some data and apply formatting to create a revision
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Apply a style to create a format revision
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Access the revision logs
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Display the revision properties
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Display style information
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


