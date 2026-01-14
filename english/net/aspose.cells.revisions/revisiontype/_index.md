---
title: Enum RevisionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionType enum. Represents the revision type
type: docs
url: /net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Represents the revision type.

```csharp
public enum RevisionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| CustomView | `0` | Custom view. |
| DefinedName | `1` | Defined name. |
| ChangeCells | `2` | Cells change. |
| AutoFormat | `3` | Auto format. |
| MergeConflict | `4` | Merge conflict. |
| Comment | `5` | Comment. |
| Format | `6` | Format. |
| InsertSheet | `7` | Insert worksheet. |
| MoveCells | `8` | Move cells. |
| Undo | `9` | Undo. |
| QueryTable | `10` | Query table. |
| InsertDelete | `11` | Inserting or deleting. |
| RenameSheet | `12` | Rename worksheet. |
| Unknown | `13` | Unknown. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrate using different RevisionType enum values
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Display enum values and their underlying integer values
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Demonstrate checking revision types
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Save the workbook
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


