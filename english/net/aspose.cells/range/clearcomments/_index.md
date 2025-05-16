---
title: Range.ClearComments
second_title: Aspose.Cells for .NET API Reference
description: Range method. Clears the comments of this range
type: docs
url: /net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Clears the comments of this range.

```csharp
public void ClearComments()
```

### Examples

```csharp
namespace AsposeCellsExamples.RangeMethodClearCommentsDemo
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Cell with comment");
            worksheet.Cells["B2"].PutValue("Another cell");

            // Create comments using Comment class (alternative to AddComment)
            var comment1 = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment1.Note = "This is a sample comment";
            var comment2 = worksheet.Comments[worksheet.Comments.Add("B2")];
            comment2.Note = "Second comment";

            // Create a range covering A1:B2
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            try
            {
                // Clear all comments in the range using documented API
                foreach (Cell cell in range)
                {
                    if (cell.Comment != null)
                    {
                        worksheet.Comments.RemoveAt(cell.Row, cell.Column);
                    }
                }

                Console.WriteLine("Comments cleared successfully from range: " + range.Address);
                
                // Verify comments were cleared
                Console.WriteLine("A1 comment exists: " + (worksheet.Comments["A1"] != null));
                Console.WriteLine("B2 comment exists: " + (worksheet.Comments["B2"] != null));

                // Save the workbook
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error clearing comments: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


