##Comment.Characters
Comment method. Returns a Characters object that represents a range of characters within the comment text
## Comment.Characters method
Returns a Characters object that represents a range of characters within the comment text.
```csharp
public FontSetting Characters(int startIndex, int length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |
### Return Value
Characters object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentMethodCharactersWithInt32Int32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment1 = worksheet.Comments[commentIndex];
comment1.Note = "This is a sample comment";
// Get font setting for first 4 characters
FontSetting fontSetting = comment1.Characters(0, 4);
// Modify the font settings
fontSetting.Font.Color = System.Drawing.Color.Red;
fontSetting.Font.IsBold = true;
// Save the workbook
workbook.Save("CommentFontSettingDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
