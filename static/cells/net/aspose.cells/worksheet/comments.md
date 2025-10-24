##Worksheet.Comments
Worksheet property. Gets the Comment collection
## Worksheet.Comments property
Gets the [`Comment`](../../comment/) collection.
```csharp
public CommentCollection Comments { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCommentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add comments to cells
worksheet.Cells["A1"].PutValue("Cell A1");
int commentIndexA1 = worksheet.Comments.Add("A1");
worksheet.Comments[commentIndexA1].Note = "Note for A1";
worksheet.Cells["B1"].PutValue("Cell B1");
int commentIndexB1 = worksheet.Comments.Add("B1");
worksheet.Comments[commentIndexB1].Note = "Note for B1";
worksheet.Cells["C2"].PutValue("Cell C2");
int commentIndexC2 = worksheet.Comments.Add("C2");
worksheet.Comments[commentIndexC2].Note = "Note for C2";
// Save the workbook
workbook.Save("CommentsDemo.xlsx");
}
}
}
```
### See Also
* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
