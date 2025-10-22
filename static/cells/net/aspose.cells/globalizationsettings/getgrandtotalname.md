##GlobalizationSettings.GetGrandTotalName
GlobalizationSettings method. Gets the grand total name of the function
## GlobalizationSettings.GetGrandTotalName method
Gets the grand total name of the function.
```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
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
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data for pivot table
CreateSampleData(worksheet);
// Instantiate custom globalization settings
var globalizationSettings = new CustomGlobalizationSettings();
try
{
// Demonstrate direct method call
string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
Console.WriteLine($"Grand Total Name: {grandTotalName}");
// Apply customization to workbook settings
workbook.Settings.GlobalizationSettings = globalizationSettings;
// Create pivot table to demonstrate effect
CreatePivotTable(worksheet);
Console.WriteLine("Method executed successfully. Check output file.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
}
// Save the result
workbook.Save("GrandTotalNameDemo.xlsx");
}
private static void CreateSampleData(Worksheet worksheet)
{
var cells = worksheet.Cells;
cells["A1"].Value = "Category";
cells["B1"].Value = "Value";
cells["A2"].Value = "Electronics";
cells["B2"].Value = 1000;
cells["A3"].Value = "Furniture";
cells["B3"].Value = 1500;
cells["A4"].Value = "Electronics";
cells["B4"].Value = 800;
}
private static void CreatePivotTable(Worksheet worksheet)
{
// Create pivot table using sample data range
int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Configure pivot table fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField dataField = pivotTable.DataFields[dataFieldIndex];
dataField.Function = ConsolidationFunction.Sum;
// Refresh table to apply settings
pivotTable.RefreshData();
pivotTable.CalculateData();
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetGrandTotalName(ConsolidationFunction functionType)
{
// Custom implementation based on consolidation function
return functionType == ConsolidationFunction.Sum
? "**[Sum Total]**"
: base.GetGrandTotalName(functionType);
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
