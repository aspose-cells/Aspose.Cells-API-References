---
title: RevisionQueryTable.CellArea
second_title: Aspose.Cells for .NET API Reference
description: RevisionQueryTable property. Gets the location of the affected query table
type: docs
url: /net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Gets the location of the affected query table.

```csharp
public CellArea CellArea { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
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
                // In a real scenario, you would get revisions from the workbook
                // For demonstration, we'll create a conceptual example
                // Note: RevisionQueryTable instances are typically obtained from workbook revisions
                RevisionQueryTable revisionQueryTable = null;

                // Check if we have a revision query table
                if (revisionQueryTable != null)
                {
                    // Display the CellArea property value (read-only)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Display other properties for context
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Save the workbook
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


