##ListColumn.Formula
ListColumn property. Gets and sets the formula of the list column
## ListColumn.Formula property
Gets and sets the formula of the list column.
```csharp
public string Formula { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnPropertyFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data and table
sheet.Cells["A1"].PutValue("Numbers");
sheet.Cells["A2"].PutValue(5);
sheet.Cells["A3"].PutValue(10);
sheet.Cells["A4"].PutValue(15);
sheet.Cells["B1"].PutValue("Doubled");
sheet.Cells["B2"].PutValue("=A2*2");
int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = sheet.ListObjects[tableIndex];
table.ShowTotals = true;
// Add formula to the list column
ListColumn column = table.ListColumns[0];
column.Formula = "=A2*3"; // This will apply to all cells in the column
// Save the workbook
workbook.Save("ListColumnFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
