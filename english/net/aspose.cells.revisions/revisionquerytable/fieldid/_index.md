---
title: RevisionQueryTable.FieldId
second_title: Aspose.Cells for .NET API Reference
description: RevisionQueryTable property. Gets ID of the specific query table field that was removed
type: docs
url: /net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Gets ID of the specific query table field that was removed.

```csharp
public int FieldId { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Create a query table (this is a simplified example)
                // Note: In a real scenario, you would need to create a query table first
                // For demonstration purposes, we'll simulate accessing a RevisionQueryTable

                // Since we can't directly create a RevisionQueryTable in this simplified example,
                // we'll demonstrate how to access the FieldId property if we had one
                // This shows the pattern for reading the read-only property

                // Simulate getting a RevisionQueryTable from revisions (conceptual)
                // In reality, you would get this from workbook.Revisions or similar
                RevisionQueryTable revisionQueryTable = null;

                // Check if we have a revision query table (this is just for demonstration)
                if (revisionQueryTable != null)
                {
                    // Display the FieldId property value
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Display other properties for context
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Save the workbook
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


