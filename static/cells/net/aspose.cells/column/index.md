##Column.Index
Column property. Gets the index of this column
## Column.Index property
Gets the index of this column.
```csharp
public int Index { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnPropertyIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to columns
worksheet.Cells["A1"].PutValue("Column 1");
worksheet.Cells["B1"].PutValue("Column 2");
worksheet.Cells["C1"].PutValue("Column 3");
// Get the column collection
ColumnCollection columns = worksheet.Cells.Columns;
// Demonstrate Index property
Console.WriteLine("Column Indices:");
for (int i = 0; i < columns.Count; i++)
{
Column column = columns[i];
Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
}
// Access column by index
Column columnB = columns[1]; // B column (index 1)
Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
// Modify column width using index
columns[2].Width = 30; // C column (index 2)
Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
