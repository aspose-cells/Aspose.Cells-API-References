##CommentCollection.Add
CommentCollection method. Adds a comment to the collection
## Add(int, int) {#add}
Adds a comment to the collection.
```csharp
public int Add(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index. |
| column | Int32 | Cell column index. |
### Return Value
[`Comment`](../../comment/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionMethodAddWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
CommentCollection comments = worksheet.Comments;
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_1}
Adds a comment to the collection.
```csharp
public int Add(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
### Return Value
[`Comment`](../../comment/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
CommentCollection comments = worksheet.Comments;
int commentIndex1 = comments.Add("A1");
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Arial";
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
