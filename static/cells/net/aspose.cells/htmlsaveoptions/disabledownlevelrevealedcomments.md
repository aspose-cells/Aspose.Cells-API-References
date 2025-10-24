##HtmlSaveOptions.DisableDownlevelRevealedComments
HtmlSaveOptions property. Indicates if disable Downlevelrevealed conditional comments when exporting file to html the default value is false
## HtmlSaveOptions.DisableDownlevelRevealedComments property
Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.
```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
{
public static void Run()
{
// Create a sample workbook with a comment
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
comment.Note = "This is a test comment";
// Set HTML save options with DisableDownlevelRevealedComments
HtmlSaveOptions options = new HtmlSaveOptions();
options.DisableDownlevelRevealedComments = true;
// Save the workbook with HTML options
workbook.Save("output.html", options);
Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
