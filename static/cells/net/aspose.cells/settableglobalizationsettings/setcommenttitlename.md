##SettableGlobalizationSettings.SetCommentTitleName
SettableGlobalizationSettings method. Gets the locale dependent comment title name according to comment title type
## SettableGlobalizationSettings.SetCommentTitleName method
Gets the locale dependent comment title name according to comment title type.
```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | CommentTitleType | type of comment title |
| name | String | locale dependent comment title name |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a sample comment";
comment.IsVisible = true;
// Create globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Set custom comment title names for different types
settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");
// Apply the globalization settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
}
}
}
```
### See Also
* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
