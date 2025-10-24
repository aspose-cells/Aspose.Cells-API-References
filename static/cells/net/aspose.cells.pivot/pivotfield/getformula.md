##PivotField.GetFormula
PivotField method. Gets formula of the calculated field
## PivotField.GetFormula method
Gets formula of the calculated field .
```csharp
public string GetFormula()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodGetFormulaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Bike";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["A3"].Value = "Car";
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["A4"].Value = "Bike";
worksheet.Cells["B4"].Value = 1500;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add calculated field with formula
pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
// Get the formula from the calculated field
PivotFieldCollection fields = pivotTable.DataFields;
string formula = fields[fields.Count - 1].GetFormula();
// Output the formula
Console.WriteLine("Calculated field formula: " + formula);
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
