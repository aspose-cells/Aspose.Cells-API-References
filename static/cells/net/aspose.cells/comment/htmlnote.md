##Comment.HtmlNote
Comment property. Gets and sets the html string which contains data and some formats in this comment
## Comment.HtmlNote property
Gets and sets the html string which contains data and some formats in this comment.
```csharp
public string HtmlNote { get; set; }
```
### Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyHtmlNoteDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
workbook.Save("CommentHtmlNoteDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
