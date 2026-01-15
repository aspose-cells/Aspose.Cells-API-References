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
            // Create a new workbook with shared mode to enable revision tracking
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data and apply formatting to create a revision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Apply a style to create a format revision
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Access the revision logs
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Display the Type property value
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Show additional information about the revision
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Save the workbook
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


