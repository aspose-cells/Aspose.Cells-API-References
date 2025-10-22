##SettableGlobalizationSettings.GetGrandTotalName
SettableGlobalizationSettings method. Gets the grand total name of the function
## SettableGlobalizationSettings.GetGrandTotalName method
Gets the grand total name of the function.
```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | ConsolidationFunction | The function type. |
### Return Value
The grand total name of the function.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot; // Added this using directive
using System;
public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set custom grand total names for different consolidation functions
settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call GetGrandTotalName with different consolidation functions
string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
// Output the results
Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);
// Create a pivot table to demonstrate the effect
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Sales");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue(1000);
cells["A3"].PutValue("Orange");
cells["B3"].PutValue(2000);
cells["A4"].PutValue("Banana");
cells["B4"].PutValue(3000);
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
// Correct way to add another data field with Average function
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
