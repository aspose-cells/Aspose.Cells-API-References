##Comment.GetCharacters
Comment method. Returns all Characters objects that represents a range of characters within the comment text
## Comment.GetCharacters method
Returns all Characters objects that represents a range of characters within the comment text.
```csharp
[Obsolete("Use Comment.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```
### Return Value
All Characters objects
### Remarks
NOTE: This method is now obsolete. Instead, please use Comment.GetRichFormattings() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentMethodGetCharactersDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a test comment with rich text formatting.";
// Get characters from the comment
ArrayList characters = comment.GetCharacters();
// Display character information
foreach (FontSetting ch in characters)
{
Console.WriteLine($"Font: {ch.Font.Name}, Size: {ch.Font.Size}");
}
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
