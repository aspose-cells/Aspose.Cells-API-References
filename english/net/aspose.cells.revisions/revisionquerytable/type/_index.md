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
            
            try
            {
                // Check if workbook has revisions (though we can't create them directly)
                if (workbook.HasRevisions)
                {
                    // In a real scenario, we would access existing revisions
                    // This demonstrates how we would check the Type property if we had access
                    Console.WriteLine("Workbook contains revisions");
                    
                    // Example of how Type property would be accessed (if we had a revision instance)
                    // RevisionQueryTable revision = GetExistingRevisionQueryTable(workbook);
                    // Console.WriteLine($"Revision Type: {revision.Type}");
                }
                else
                {
                    // Since we can't create revisions directly, we'll demonstrate the enum values
                    Console.WriteLine("Available RevisionType values:");
                    foreach (RevisionType type in Enum.GetValues(typeof(RevisionType)))
                    {
                        Console.WriteLine($"- {type} ({(int)type})");
                    }
                    
                    // QueryTable is one of the RevisionType values (value 10)
                    Console.WriteLine("\nThe QueryTable revision type is: " + RevisionType.QueryTable);
                }

                // Save the workbook
                workbook.Save("RevisionQueryTableTypeDemo.xlsx");
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


