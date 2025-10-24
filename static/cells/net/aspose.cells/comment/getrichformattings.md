##Comment.GetRichFormattings
Comment method. Returns all Characters objects that represents a range of characters within the comment text
## Comment.GetRichFormattings method
Returns all Characters objects that represents a range of characters within the comment text.
```csharp
public FontSetting[] GetRichFormattings()
```
### Return Value
All Characters objects
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentMethodGetRichFormattingsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";
// Get rich text formattings
FontSetting[] formattings = comment.GetRichFormattings();
// Display formatting information
Console.WriteLine("Rich Text Formattings:");
foreach (FontSetting setting in formattings)
{
Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
}
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
