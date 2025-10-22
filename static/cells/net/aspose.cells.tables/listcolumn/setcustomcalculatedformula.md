##ListColumn.SetCustomCalculatedFormula
ListColumn method. Sets the formula for this list column
## ListColumn.SetCustomCalculatedFormula method
Sets the formula for this list column.
```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | the formula for this list column. |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["B1"].PutValue("Total");
// Create table
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
ListObject table = worksheet.ListObjects[tableIndex];
// Get second list column
ListColumn totalColumn = table.ListColumns[1];
try
{
// Set custom formula using A1 notation with standard locale
totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
Console.WriteLine("Custom formula set successfully.");
Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
