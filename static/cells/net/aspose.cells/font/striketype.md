##Font.StrikeType
Font property. Gets the strike type of the text
## Font.StrikeType property
Gets the strike type of the text.
```csharp
public TextStrikeType StrikeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyStrikeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a cell with rich text
cells["A1"].PutValue("Sample Text");
// Access the rich text formatting
FontSetting fontSetting = cells["A1"].GetCharacters()[0];
// Set strike type to single
fontSetting.Font.StrikeType = TextStrikeType.Single;
// Verify the strike type
Console.WriteLine("Strike Type: " + fontSetting.Font.StrikeType);
// Save the workbook
workbook.Save("FontPropertyStrikeTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextStrikeType](../../textstriketype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
