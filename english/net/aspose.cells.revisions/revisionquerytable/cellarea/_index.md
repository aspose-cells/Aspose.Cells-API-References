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
namespace AsposeCellsExamples.RevisionQueryTablePropertyCellAreaDemo
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
            
            try
            {
                // Check if workbook has revisions
                if (workbook.HasRevisions)
                {
                    // In a real scenario, we would access existing RevisionQueryTable instances
                    // This demonstrates how we would check the CellArea property if we had access
                    Console.WriteLine("Workbook contains revisions");
                    
                    // Example of how CellArea property would be accessed (if we had a revision instance)
                    // RevisionQueryTable revision = GetExistingRevisionQueryTable(workbook);
                    // Console.WriteLine($"Query Table Cell Area: {revision.CellArea}");
                }
                else
                {
                    // Since we can't create revisions directly, we'll demonstrate the CellArea structure
                    Console.WriteLine("Creating a sample CellArea to demonstrate the structure:");
                    
                    // Create a sample CellArea using the static CreateCellArea method
                    CellArea area = CellArea.CreateCellArea(0, 0, 5, 3);
                    Console.WriteLine($"Sample CellArea: {area}");
                    
                    // Show how the CellArea would be accessed from a RevisionQueryTable
                    Console.WriteLine("\nIn a RevisionQueryTable, the CellArea property would show the affected query table location");
                }

                // Save the workbook
                workbook.Save("RevisionQueryTableCellAreaDemo.xlsx");
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


