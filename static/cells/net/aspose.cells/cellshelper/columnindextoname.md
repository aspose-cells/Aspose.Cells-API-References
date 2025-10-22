##CellsHelper.ColumnIndexToName
CellsHelper method. Gets column name according to column index
## CellsHelper.ColumnIndexToName method
Gets column name according to column index.
```csharp
public static string ColumnIndexToName(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
### Return Value
Name of column.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodColumnIndexToNameWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values in cells to demonstrate column index to name conversion
worksheet.Cells["A1"].PutValue("Column Index");
worksheet.Cells["B1"].PutValue("Column Name");
// Demonstrate ColumnIndexToName for indices 0-4
for (int i = 0; i < 5; i++)
{
worksheet.Cells[i + 1, 0].PutValue(i);
string columnName = CellsHelper.ColumnIndexToName(i);
worksheet.Cells[i + 1, 1].PutValue(columnName);
}
// Save the workbook
workbook.Save("ColumnIndexToNameDemo.xlsx");
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
