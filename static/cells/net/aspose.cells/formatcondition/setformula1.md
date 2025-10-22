##FormatCondition.SetFormula1
FormatCondition method. Sets the value or expression associated with this format condition
## FormatCondition.SetFormula1 method
Sets the value or expression associated with this format condition.
```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add a conditional formatting range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 3;
area.EndColumn = 0;
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
// Get the first format condition
FormatCondition fc = fcc[0];
try
{
// Call SetFormula1 with parameters (String, Boolean, Boolean)
fc.SetFormula1("SUM(A1:A4)", false, false);
// Display the result
Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
}
// Save the result
workbook.Save("FormatConditionSetFormula1Demo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
