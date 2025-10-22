##Cell.GetTable
Cell method. Gets the table which contains this cell
## Cell.GetTable method
Gets the table which contains this cell.
```csharp
public ListObject GetTable()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class CellMethodGetTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a table with headers and data
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue(2.5);
cells["A3"].PutValue("Orange");
cells["B3"].PutValue(1.8);
// Create a ListObject (table) from the data range
int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
ListObject table = worksheet.ListObjects[tableIndex];
// Demonstrate GetTable method
Cell cellInTable = cells["B2"];
ListObject resultTable = cellInTable.GetTable();
Console.WriteLine("Table found: " + (resultTable != null));
Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn +
" to " + resultTable.EndRow + "," + resultTable.EndColumn);
}
}
}
```
### See Also
* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
