##Aspose::Cells::Drawing::ShapeCollection::CopyCommentsInRange method
'Aspose::Cells::Drawing::ShapeCollection::CopyCommentsInRange method. Copy all comments in the range in C++.'
## ShapeCollection::CopyCommentsInRange method
Copy all comments in the range.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::CopyCommentsInRange(const ShapeCollection &shapes, const CellArea &ca, int32_t destRow, int32_t destColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| shapes | const ShapeCollection\& | The source shapes. |
| ca | const CellArea\& | The source range. |
| destRow | int32_t | The dest range start row. |
| destColumn | int32_t | The dest range start column. |
## Examples
```cpp
CommentCollection comments = workbook.GetWorksheets().Get(0).GetComments();
//Add comment to cell A1
int commentIndex = comments.Add(0, 0);
Comment comment = comments.Get(commentIndex);
comment.SetNote(u"First note.");
comment.GetFont().SetName(u"Times New Roman");
//Add comment to cell B2
comments.Add("B2");
comment = comments.Get(u"B2");
comment.SetNote(u"Second note.");
CellArea area1;
area1.StartColumn = 1;
area1.StartRow = 1;
area1.EndColumn = 5;
area1.EndRow = 4;
//copy
shapeCollection.CopyCommentsInRange(shapeCollection, area1, 5, 1);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Class [CellArea](../../../aspose.cells/cellarea/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
