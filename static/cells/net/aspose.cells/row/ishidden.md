##Row.IsHidden
Row property. Indicates whether the row is hidden
## Row.IsHidden property
Indicates whether the row is hidden.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyIsHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
for (int i = 0; i < 10; i++)
{
cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
}
// Hide some rows
cells.HideRow(2);  // Row 3 (0-based index 2)
cells.HideRow(5);  // Row 6 (0-based index 5)
cells.HideRow(8);  // Row 9 (0-based index 8)
// Check and display IsHidden status for each row
for (int i = 0; i < 10; i++)
{
bool isHidden = cells.Rows[i].IsHidden;
Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
}
// Save the workbook
workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
