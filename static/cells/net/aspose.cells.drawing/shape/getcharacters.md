##Shape.GetCharacters
Shape method. Returns all Characters objects that represents a range of characters within the text
## Shape.GetCharacters method
Returns all Characters objects that represents a range of characters within the text .
```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```
### Return Value
All Characters objects
### Remarks
NOTE: This method is now obsolete. Instead, please use Shape.GetRichFormattings() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetCharactersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape to the worksheet with all required parameters
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
shape.Text = "Sample Text";
// Get the characters from the shape
ArrayList characters = shape.GetCharacters();
// Display information about each character
foreach (FontSetting charSetting in characters)
{
Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
