##SettablePivotGlobalizationSettings.SetTextOfAll
SettablePivotGlobalizationSettings method. Sets the text of All label in the PivotTable
## SettablePivotGlobalizationSettings.SetTextOfAll method
Sets the text of "(All)" label in the PivotTable.
```csharp
public void SetTextOfAll(string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Create pivot table
var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
var pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create globalization settings
var settings = new SettableGlobalizationSettings();
settings.PivotSettings = new SettablePivotGlobalizationSettings();
try
{
// Call SetTextOfAll method to change "(All)" text
((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
}
// Save the result
workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
}
}
}
```
### See Also
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
