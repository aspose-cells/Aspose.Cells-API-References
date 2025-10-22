##Cells.Columns
Cells property. Gets the collection of Column objects that represents the individual columns in this worksheet
## Cells.Columns property
Gets the collection of [`Column`](../../column/) objects that represents the individual columns in this worksheet.
```csharp
public ColumnCollection Columns { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyColumnsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set style for column 5
Style columnStyle = workbook.CreateStyle();
columnStyle.Font.Name = "Arial";
columnStyle.Font.Size = 12;
columnStyle.Font.IsBold = true;
cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });
// Set width for column 5
cells.Columns[5].Width = 20;
// Set data in column 5 to demonstrate the style
for (int row = 0; row < 10; row++)
{
cells[row, 5].PutValue($"Row {row + 1}");
}
// Save the workbook
workbook.Save("ColumnsPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
