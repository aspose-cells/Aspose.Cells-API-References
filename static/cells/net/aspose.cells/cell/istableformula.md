##Cell.IsTableFormula
Cell property. Indicates whether this cell is part of table formula
## Cell.IsTableFormula property
Indicates whether this cell is part of table formula.
```csharp
public bool IsTableFormula { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class CellPropertyIsTableFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a table
int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
ListObject table = worksheet.ListObjects[index];
// Add table formula to cell D2
Cell cell = worksheet.Cells["D2"];
cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
// Check if the cell contains a table formula
Console.WriteLine("Is table formula: " + cell.IsTableFormula);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
