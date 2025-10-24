##GlobalizationSettings.GetCommentTitleName
GlobalizationSettings method. Gets the locale dependent comment title name according to comment title type
## GlobalizationSettings.GetCommentTitleName method
Gets the locale dependent comment title name according to comment title type.
```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | CommentTitleType |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
{
public override string GetCommentTitleName(CommentTitleType type)
{
switch (type)
{
case CommentTitleType.Cell:
return "Custom Cell Comment";
case CommentTitleType.Reply:  // Changed from Threaded to Reply
return "Custom Threaded Comment";
default:
return base.GetCommentTitleName(type);
}
}
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings
Worksheet worksheet = workbook.Worksheets[0];
// Add test comment
int commentIndex = worksheet.Comments.Add("B5");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Test comment content";
try
{
// Get comment title for different types
var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings
Console.WriteLine($"Cell Comment Title: {cellTitle}");
Console.WriteLine($"Threaded Comment Title: {threadedTitle}");
// Set comment author (title) using our custom globalization settings
comment.Author = cellTitle; // Changed from Title to Author
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
}
workbook.Save("GetCommentTitleNameDemo.xlsx");
}
}
}
```
### See Also
* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
