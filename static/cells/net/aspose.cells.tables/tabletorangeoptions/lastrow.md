##TableToRangeOptions.LastRow
TableToRangeOptions property. Gets and sets the last row index of the table
## TableToRangeOptions.LastRow property
Gets and sets the last row index of the table.
```csharp
public int LastRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableToRangeOptionsPropertyLastRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 5; col++)
{
cells[row, col].PutValue($"Data {row}-{col}");
}
}
// Create table
int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;
// Convert table to range with LastRow specified
TableToRangeOptions options = new TableToRangeOptions
{
LastRow = 7 // Only convert rows 0-7 (excluding 8-9)
};
table.ConvertToRange(options);
workbook.Save("TableToRangeWithLastRow.xlsx");
}
}
}
```
### See Also
* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
