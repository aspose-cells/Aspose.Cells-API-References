##SettableGlobalizationSettings.GetCommentTitleName
SettableGlobalizationSettings method. Gets the locale dependent comment title name according to comment title type
## SettableGlobalizationSettings.GetCommentTitleName method
Gets the locale dependent comment title name according to comment title type.
```csharp
public override string GetCommentTitleName(CommentTitleType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | CommentTitleType | type of comment title |
### Return Value
locale dependent comment title name
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a comment in cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a test comment";
comment.IsVisible = true;
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set custom comment title names for different types
settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");
// Apply the globalization settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Get and display the comment title names
Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
}
// Save the workbook
workbook.Save("CommentTitleNamesDemo.xlsx");
}
}
}
```
### See Also
* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
