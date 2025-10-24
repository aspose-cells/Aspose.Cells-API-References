##SettableGlobalizationSettings.SetGrandTotalName
SettableGlobalizationSettings method. Sets the grand total name of specific function
## SettableGlobalizationSettings.SetGrandTotalName method
Sets the grand total name of specific function.
```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | The function type. |
| name | String | The grand total name of the function. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Fruit");
worksheet.Cells["A4"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(75);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call SetGrandTotalName with ConsolidationFunction.Sum and custom name
settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");
// Refresh pivot table to apply changes
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
