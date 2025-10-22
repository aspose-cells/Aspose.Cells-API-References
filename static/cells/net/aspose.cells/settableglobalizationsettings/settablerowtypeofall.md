##SettableGlobalizationSettings.SetTableRowTypeOfAll
SettableGlobalizationSettings method. Sets the type name of table rows that consists of all rows in referenced table
## SettableGlobalizationSettings.SetTableRowTypeOfAll method
Sets the type name of table rows that consists of all rows in referenced table.
```csharp
public void SetTableRowTypeOfAll(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for a table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue(2.5);
cells["A3"].PutValue("Orange");
cells["B3"].PutValue(1.8);
// Create a table
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Call SetTableRowTypeOfAll with custom name
settings.SetTableRowTypeOfAll("CompleteTable");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Verify the setting by getting the value back
string rowType = settings.GetTableRowTypeOfAll();
Console.WriteLine($"Table row type for all rows set to: {rowType}");
// Add a formula that references all rows using the custom name
cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");
// Calculate formulas
workbook.CalculateFormula();
Console.WriteLine($"Calculation result: {cells["C2"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
