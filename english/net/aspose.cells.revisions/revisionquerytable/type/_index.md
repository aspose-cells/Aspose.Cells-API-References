---
title: RevisionQueryTable.Type
second_title: Aspose.Cells for .NET API Reference
description: RevisionQueryTable property. Represents the type of the revision
type: docs
url: /net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Represents the type of the revision.

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

    public class RevisionQueryTablePropertyTypeDemo
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

                // Create a mock RevisionQueryTable (this is conceptual - in reality you'd get from revisions)
                // Since we can't directly instantiate RevisionQueryTable, we'll demonstrate the pattern
                RevisionQueryTable revisionQueryTable = null;

                // Check if we have a revision query table
                if (revisionQueryTable != null)
                {
                    // Display the Type property value (read-only)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Show the enum value as integer for reference
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Display other properties for context
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Save the workbook
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


