---
title: ShapeCollection.CopyCommentsInRange
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Copy all comments in the range
type: docs
url: /net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
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

[C#]
CommentCollection comments = workbook.Worksheets[0].Comments;

//Add comment to cell A1
int commentIndex = comments.Add(0, 0);
Comment comment = comments[commentIndex];
comment.Note = "First note.";
comment.Font.Name = "Times New Roman";

//Add comment to cell B2
comments.Add("B2");
comment = comments["B2"];
comment.Note = "Second note.";

CellArea area1 = new CellArea();
area1.StartColumn = 1;
area1.StartRow = 1;
area1.EndColumn = 5;
area1.EndRow = 4;

//copy
shapes.CopyCommentsInRange(shapes, area1, 5, 1);

```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


