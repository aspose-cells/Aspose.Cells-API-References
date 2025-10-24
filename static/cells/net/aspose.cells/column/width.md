##Column.Width
Column property. Gets and sets the column width in unit of characters
## Column.Width property
Gets and sets the column width in unit of characters.
```csharp
public double Width { get; set; }
```
### Remarks
For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnPropertyWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set width for column 3 (index 2)
worksheet.Cells.Columns[2].Width = 25.5;
// Set width for column 4 (index 3)
worksheet.Cells.Columns[3].Width = 40.0;
// Get and display the widths
Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
// Save the workbook
workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
