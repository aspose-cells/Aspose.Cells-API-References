##SettableGlobalizationSettings.SetTableRowTypeOfCurrent
SettableGlobalizationSettings method. Sets the type name of table rows that consists of the current row in referenced table
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method
Sets the type name of table rows that consists of the current row in referenced table.
```csharp
public void SetTableRowTypeOfCurrent(string name)
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
public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue("2.5");
cells["A3"].PutValue("Banana");
cells["B3"].PutValue("1.5");
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowTotals = true;
table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
// Create globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Set custom name for current row type
settings.SetTableRowTypeOfCurrent("CurrentItem");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Verify the setting by getting the value back
string currentRowType = settings.GetTableRowTypeOfCurrent();
Console.WriteLine($"Current row type name set to: {currentRowType}");
// Save the workbook
workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
}
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
