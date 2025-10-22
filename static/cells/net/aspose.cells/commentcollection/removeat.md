##CommentCollection.RemoveAt
CommentCollection method. Removes the comment of the specific cell
## RemoveAt(string) {#removeat_2}
Removes the comment of the specific cell.
```csharp
public void RemoveAt(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of cell which contains a comment. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionMethodRemoveAtWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells using cell names
int commentIndex1 = worksheet.Comments.Add("A1");
worksheet.Comments[commentIndex1].Note = "Comment in A1";
int commentIndex2 = worksheet.Comments.Add("B2");
worksheet.Comments[commentIndex2].Note = "Comment in B2";
int commentIndex3 = worksheet.Comments.Add("C3");
worksheet.Comments[commentIndex3].Note = "Comment in C3";
// Remove comment at cell B2 using RemoveAt with string parameter
worksheet.Comments.RemoveAt("B2");
// Save the workbook
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveAt(int, int) {#removeat_1}
Removes the comment of the specific cell.
```csharp
public void RemoveAt(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | the column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells using cell references
int comment1Index = worksheet.Comments.Add("A1");
worksheet.Comments[comment1Index].Note = "First comment";
int comment2Index = worksheet.Comments.Add("B2");
worksheet.Comments[comment2Index].Note = "Second comment";
int comment3Index = worksheet.Comments.Add("C3");
worksheet.Comments[comment3Index].Note = "Third comment";
// Remove comment at row 1, column 1 (B2)
worksheet.Comments.RemoveAt(1, 1);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
