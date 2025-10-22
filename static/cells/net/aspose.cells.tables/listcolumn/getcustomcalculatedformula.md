##ListColumn.GetCustomCalculatedFormula
ListColumn method. Gets the formula of this list column
## ListColumn.GetCustomCalculatedFormula method
Gets the formula of this list column.
```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The formula of this list column.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["A3"].PutValue("Mary");
sheet.Cells["B1"].PutValue("Score");
sheet.Cells["B2"].PutValue(85);
sheet.Cells["B3"].PutValue(92);
// Create a list object
int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = sheet.ListObjects[index];
// Add a calculated column
ListColumn calcColumn = listObject.ListColumns[1];
calcColumn.Formula = "=WEEKNUM([@Score])";
// Get the custom calculated formula
string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
// Output the result
Console.WriteLine("Calculated Formula: " + formula);
}
}
}
```
### See Also
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
