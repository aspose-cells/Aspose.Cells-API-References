##FormatCondition.SetFormula2
FormatCondition method. Sets the value or expression associated with this format condition
## FormatCondition.SetFormula2 method
Sets the value or expression associated with this format condition.
```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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
public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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
// Add a format condition
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 3;
area.StartColumn = 0;
area.EndColumn = 0;
fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
// Get the first format condition
FormatCondition fc = fcs[0];
try
{
// Call SetFormula2 with parameters (String, Boolean, Boolean)
fc.SetFormula2("25", false, false);
// Display the result
Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");
// Apply some style to make the effect visible
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.LightGreen;
fc.Style = style;
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
}
// Save the result
workbook.Save("FormatConditionSetFormula2Demo.xlsx");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
