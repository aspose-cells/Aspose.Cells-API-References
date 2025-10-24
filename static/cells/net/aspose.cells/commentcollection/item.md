##CommentCollection.Item
CommentCollection property. Gets the Comment element at the specified index
## CommentCollection indexer (1 of 3)
Gets the [`Comment`](../../comment/) element at the specified index.
```csharp
public Comment this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells
int commentIndex1 = worksheet.Comments.Add("A1");
int commentIndex2 = worksheet.Comments.Add("B2");
// Access comments using Item property
Comment comment1 = worksheet.Comments[commentIndex1];
Comment comment2 = worksheet.Comments[commentIndex2];
// Set comment notes
comment1.Note = "First comment";
comment2.Note = "Second comment";
// Modify first comment using Item property
worksheet.Comments[0].Note = "Updated first comment";
// Access and modify comment directly from collection
Comment comment3 = worksheet.Comments[1];
comment3.Note = "Updated second comment";
// Save the workbook
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CommentCollection indexer (2 of 3)
Gets the [`Comment`](../../comment/) element at the specified cell.
```csharp
public Comment this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name. |
### Return Value
The element at the specified cell.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionPropertyItemDemo2
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells using cell references
int comment1Index = worksheet.Comments.Add(0, 0); // A1
worksheet.Comments[comment1Index].Note = "First comment";
int comment2Index = worksheet.Comments.Add(1, 1); // B2
worksheet.Comments[comment2Index].Note = "Second comment";
int comment3Index = worksheet.Comments.Add(2, 2); // C3
worksheet.Comments[comment3Index].Note = "Third comment";
// Access comments using Item property with cell references
CommentCollection comments = worksheet.Comments;
Comment comment1 = comments["A1"];
Comment comment2 = comments["B2"];
Comment comment3 = comments["C3"];
// Modify comment notes
comment1.Note = "Updated first note";
comment2.Note = "Updated second note";
comment3.Note = "Updated third note";
// Save the workbook
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CommentCollection indexer (3 of 3)
Gets the [`Comment`](../../comment/) element at the specified row index and column index.
```csharp
public Comment this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |
### Return Value
The element at the specified cell.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells using cell references
int comment1Index = worksheet.Comments.Add("A1");
worksheet.Comments[comment1Index].Note = "First comment";
int comment2Index = worksheet.Comments.Add("B2");
worksheet.Comments[comment2Index].Note = "Second comment";
int comment3Index = worksheet.Comments.Add("C3");
worksheet.Comments[comment3Index].Note = "Third comment";
// Access comments using Item property with row/column indices
CommentCollection comments = worksheet.Comments;
Comment comment1 = comments[0, 0];
comment1.Note = "Updated first comment";
Comment comment2 = comments[1, 1];
comment2.Note = "Updated second comment";
// Save the workbook
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
