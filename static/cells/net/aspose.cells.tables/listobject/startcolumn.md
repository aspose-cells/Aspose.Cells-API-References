##ListObject.StartColumn
ListObject property. Gets the start column of the range
## ListObject.StartColumn property
Gets the start column of the range.
```csharp
public int StartColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyStartColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for the table
worksheet.Cells["E5"].PutValue("ID");
worksheet.Cells["F5"].PutValue("Name");
worksheet.Cells["G5"].PutValue("Age");
worksheet.Cells["E6"].PutValue(1);
worksheet.Cells["F6"].PutValue("John");
worksheet.Cells["G6"].PutValue(30);
worksheet.Cells["E7"].PutValue(2);
worksheet.Cells["F7"].PutValue("Alice");
worksheet.Cells["G7"].PutValue(25);
// Create a list object (table)
int startRow = 5;
int startCol = 4; // Column E (0-based index 4)
int endRow = 7;
int endCol = 6; // Column G (0-based index 6)
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(startRow, startCol, endRow, endCol, true)];
// Demonstrate StartColumn property
Console.WriteLine("Table starts at column index: " + table.StartColumn);
Console.WriteLine("Table starts at column letter: " + CellsHelper.ColumnIndexToName(table.StartColumn));
// Save the workbook
workbook.Save("ListObjectStartColumnDemo.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
