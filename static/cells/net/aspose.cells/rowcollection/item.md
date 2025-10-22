##RowCollection.Item
RowCollection property. Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before
## RowCollection indexer
Gets a [`Row`](../../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before.
```csharp
public Row this[int rowIndex] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set standard width for columns
cells.StandardWidth = 20.0;
// Access and style rows using Item property
for (int i = 0; i < 5; i++)
{
Row row = cells.Rows[i]; // Using Item property
Style rowStyle = workbook.CreateStyle();
rowStyle.Font.IsBold = true;
rowStyle.Font.Color = System.Drawing.Color.Blue;
row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
// Access and style cell in the row
Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
cell.PutValue($"Row {i}, Col {i}");
Style cellStyle = workbook.CreateStyle();
cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
cell.SetStyle(cellStyle);
}
// Save the workbook
workbook.Save("RowCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
