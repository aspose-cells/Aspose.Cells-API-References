##Cell.IsRichText
Cell method. Indicates whether the string value of this cell is a rich formatted text
## Cell.IsRichText method
Indicates whether the string value of this cell is a rich formatted text.
```csharp
public bool IsRichText()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodIsRichTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a cell with rich text formatting
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Hello World");
// Apply rich text formatting
FontSetting boldFont = cell.GetCharacters()[0];
boldFont.Font.IsBold = true;
FontSetting normalFont = cell.GetCharacters()[6];
normalFont.Font.IsBold = false;
// Check if the cell contains rich text
bool isRichText = cell.IsRichText();
Console.WriteLine("Is cell A1 rich text? " + isRichText);
// Save the workbook
workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
