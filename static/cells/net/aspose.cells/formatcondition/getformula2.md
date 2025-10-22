##FormatCondition.GetFormula2
FormatCondition method. Gets the value or expression associated with this format condition
## GetFormula2(bool, bool) {#getformula2}
Gets the value or expression associated with this format condition.
```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The value or expression associated with this format condition.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
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
// Add a format condition
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 2;
area.StartColumn = 0;
area.EndColumn = 0;
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
FormatCondition fc = fcs[conditionIndex];
// Set Formula2
fc.Formula2 = "30";
try
{
// Call GetFormula2 with (Boolean, Boolean) parameters
string formula2 = fc.GetFormula2(false, false);
// Display the result
Console.WriteLine("Formula2: " + formula2);
Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
}
// Save the result
workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetFormula2(bool, bool, int, int) {#getformula2_1}
Gets the value or expression of the conditional formatting of the cell.
```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
The value or expression associated with the conditional formatting of the cell.
### Remarks
The given cell must be contained by this conditional formatting, otherwise null will be returned.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
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
// Add a conditional format
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
FormatCondition fc = fcs[conditionIndex];
try
{
// Call GetFormula2 with specific parameters (isR1C1, isLocal, row, column)
string formula = fc.GetFormula2(false, false, 0, 0);
Console.WriteLine("Formula2 retrieved successfully: " + formula);
Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
}
// Save the result
workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetFormula2(int, int) {#getformula2_2}
Gets the formula of the conditional formatting of the cell.
```csharp
public string GetFormula2(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
The formula.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionMethodGetFormula2WithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["A2"].PutValue(15);
worksheet.Cells["A3"].PutValue(25);
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 1;
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");
// Get the first format condition
FormatCondition fc = fcc[0];
try
{
// Call GetFormula2 with specific row and column parameters
string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
Console.WriteLine("Formula2 for cell (1,0): " + formula);
Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
// Apply style to visualize the conditional formatting
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
fc.Style = style;
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
}
// Save the result
workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
