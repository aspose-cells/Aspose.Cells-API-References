##ColumnCollection.Item
ColumnCollection property. Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before
## ColumnCollection indexer
Gets a [`Column`](../../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.
```csharp
public Column this[int columnIndex] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access columns collection
ColumnCollection columns = worksheet.Cells.Columns;
// Set width for columns using Item property
columns[0].Width = 10;
columns[1].Width = 15;
columns[2].Width = 20;
// Display column widths
Console.WriteLine("Column 0 Width: " + columns[0].Width);
Console.WriteLine("Column 1 Width: " + columns[1].Width);
Console.WriteLine("Column 2 Width: " + columns[2].Width);
// Verify column widths are set correctly
if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
{
throw new Exception("Column widths were not set correctly");
}
}
}
}
```
### See Also
* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
