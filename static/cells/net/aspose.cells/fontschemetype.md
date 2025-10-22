##Enum FontSchemeType
Aspose.Cells.FontSchemeType enum. Represents the scheme type of the font
## FontSchemeType enumeration
Represents the scheme type of the font.
```csharp
public enum FontSchemeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None |
| Major | `1` | Major scheme. |
| Minor | `2` | Minor scheme. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontSchemeTypeDemo
{
public static void FontSchemeTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Obtain the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Accessing the "A1" cell from the worksheet
Cell cell = worksheet.Cells["A1"];
// Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!");
// Access the font of the cell style
Aspose.Cells.Font font = cell.GetStyle().Font;
// Setting the font scheme type to Major
font.SchemeType = FontSchemeType.Major;
// Setting other font properties for demonstration
font.Name = "Arial";
font.Size = 14;
font.Color = System.Drawing.Color.Blue;
// Save the workbook
workbook.Save("FontSchemeTypeExample.xlsx");
workbook.Save("FontSchemeTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
