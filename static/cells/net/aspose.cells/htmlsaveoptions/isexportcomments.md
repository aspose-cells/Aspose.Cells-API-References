##HtmlSaveOptions.IsExportComments
HtmlSaveOptions property. Indicates if exporting comments when saving file to html the default value is false
## HtmlSaveOptions.IsExportComments property
Indicates if exporting comments when saving file to html, the default value is false.
```csharp
public bool IsExportComments { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsExportCommentsDemo
{
public static void Run()
{
// Create a workbook with sample data and comments
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Data");
// Add a comment
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a test comment";
// Save with IsExportComments = false (comments won't be exported)
HtmlSaveOptions options1 = new HtmlSaveOptions
{
IsExportComments = false
};
workbook.Save("output_without_comments.html", options1);
// Save with IsExportComments = true (comments will be exported)
HtmlSaveOptions options2 = new HtmlSaveOptions
{
IsExportComments = true
};
workbook.Save("output_with_comments.html", options2);
Console.WriteLine("HTML files created successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
