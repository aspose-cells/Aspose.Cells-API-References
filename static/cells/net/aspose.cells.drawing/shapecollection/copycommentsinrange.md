##ShapeCollection.CopyCommentsInRange
ShapeCollection method. Copy all comments in the range
## ShapeCollection.CopyCommentsInRange method
Copy all comments in the range.
```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| shapes | ShapeCollection | The source shapes. |
| ca | CellArea | The source range. |
| destRow | Int32 | The dest range start row. |
| destColumn | Int32 | The dest range start column. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodCopyCommentsInRangeWithShapeCollectionCellAreaInt32InDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add comments
CommentCollection comments = worksheet.Comments;
// Add comment to cell A1
int commentIndex = comments.Add(0, 0);
Comment comment = comments[commentIndex];
comment.Note = "First note.";
comment.Font.Name = "Times New Roman";
// Add comment to cell B2
comments.Add("B2");
comment = comments["B2"];
comment.Note = "Second note.";
// Define source range
CellArea sourceArea = new CellArea();
sourceArea.StartRow = 0;
sourceArea.StartColumn = 0;
sourceArea.EndRow = 1;
sourceArea.EndColumn = 1;
// Get shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Copy comments from source range to destination (starting at row 5, column 1)
shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
