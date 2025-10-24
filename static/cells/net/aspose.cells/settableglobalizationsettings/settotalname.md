##SettableGlobalizationSettings.SetTotalName
SettableGlobalizationSettings method. Sets the total name of specific function
## SettableGlobalizationSettings.SetTotalName method
Sets the total name of specific function.
```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | The function type. |
| name | String | The total name of the function. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for consolidation
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["A4"].PutValue("Total");
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Set custom total name for Sum function
settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
// Set custom total name for Average function
settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Verify the settings by getting the values back
string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);
Console.WriteLine($"Sum total name set to: {sumTotalName}");
Console.WriteLine($"Average total name set to: {avgTotalName}");
// Create a pivot table to demonstrate the effect
worksheet.Cells["D1"].PutValue("Pivot Table");
var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
var pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("SetTotalNameDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
