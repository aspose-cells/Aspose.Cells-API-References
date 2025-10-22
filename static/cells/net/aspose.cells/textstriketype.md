##Enum TextStrikeType
Aspose.Cells.TextStrikeType enum. This type specifies the strike type
## TextStrikeType enumeration
This type specifies the strike type.
```csharp
public enum TextStrikeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Single | `0` | A single strikethrough applied on the text. |
| Double | `1` | A double strikethrough applied on the text. Only works for the text of the shapes or charts. |
| None | `2` | No strike is applied to the text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class TextStrikeTypeDemo
{
public static void TextStrikeTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Obtain the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Accessing the "A1" cell from the worksheet
Cell cell = worksheet.Cells["A1"];
// Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!");
// Accessing the font of the cell
Style style = cell.GetStyle();
Font font = style.Font;
// Setting the strike type to Single
font.StrikeType = TextStrikeType.Single;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("TextStrikeTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
