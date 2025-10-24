##SettableGlobalizationSettings.GetTotalName
SettableGlobalizationSettings method. Gets the total name of specific function
## SettableGlobalizationSettings.GetTotalName method
Gets the total name of specific function.
```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | The function type. |
### Return Value
The total name of the function.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
try
{
// Call GetTotalName with ConsolidationFunction.Sum
string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
// Display the result
Console.WriteLine($"Total name for Sum function: {totalName}");
// Add data to demonstrate the effect (though GetTotalName doesn't modify the spreadsheet)
worksheet.Cells["A1"].PutValue("Values");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["B1"].PutValue("Total");
worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
// Calculate formulas
workbook.CalculateFormula();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
