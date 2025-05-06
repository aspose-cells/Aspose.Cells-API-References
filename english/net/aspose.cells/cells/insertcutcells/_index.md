---
title: Cells.InsertCutCells
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Insert cut range
type: docs
url: /net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Insert cut range.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Int32 | The row. |
| column | Int32 | The column. |
| shiftType | ShiftType | The shift type . |

### Examples

```csharp
// Called: worksheet.Cells.InsertCutCells(sourceRange, destinationRange.FirstRow, destinationRange.FirstColumn, ShiftType.Down);
[Test]
        public void Method_ShiftType_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some notes to cells
            AddNotesToCells(worksheet);
         
            // Define the range to cut
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange($&quot;{worksheet.Name}!1:2&quot;);

            // Define the destination cell
            //Cell destCell = worksheet.Cells[&quot;A4&quot;];

            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange($&quot;{worksheet.Name}!4:4&quot;);

            // Perform the insert cut cells operation
            worksheet.Cells.InsertCutCells(sourceRange, destinationRange.FirstRow, destinationRange.FirstColumn, ShiftType.Down);

            for(int r = 1; r &lt; 3; r++)
            {
                for (int c = 0; c &lt; 2; c++)
                {
                    Cell cell = worksheet.Cells[r, c];
                    Comment comment = cell.Comment;
                    Assert.AreEqual(&quot;Note for &quot; + CellsHelper.CellIndexToName(r - 1, c),comment.Note);
                }

            }
            // Save the workbook to see the results
            workbook.Save(Constants.destPath + &quot;CellsNet55944.xlsx&quot;);
        }
```

### See Also

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


