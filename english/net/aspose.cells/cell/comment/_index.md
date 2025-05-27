---
title: Cell.Comment
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the comment of this cell
type: docs
url: /net/aspose.cells/cell/comment/
---
## Cell.Comment property

Gets the comment of this cell.

```csharp
public Comment Comment { get; }
```

### Remarks

If there is no comment applies to the cell, returns null.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access cell A1
            Cell cell = worksheet.Cells["A1"];
            
            // Add a comment to the cell using the correct API
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.Author = "Author";
            
            // Modify comment properties
            comment.Note = "Updated comment text";
            comment.Font.Name = "Arial";
            comment.Font.Size = 10;
            comment.IsVisible = true;
            
            // Save the workbook
            workbook.Save("CellCommentDemo.xlsx");
        }
    }
}
```

### See Also

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


