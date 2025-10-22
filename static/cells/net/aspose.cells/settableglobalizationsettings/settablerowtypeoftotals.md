##SettableGlobalizationSettings.SetTableRowTypeOfTotals
SettableGlobalizationSettings method. Sets the type name of table rows that consists of the total row of referenced table
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method
Sets the type name of table rows that consists of the total row of referenced table.
```csharp
public void SetTableRowTypeOfTotals(string name)
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
public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
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
cells["B2"].PutValue(10);
cells["A3"].PutValue("Orange");
cells["B3"].PutValue(15);
cells["A4"].PutValue("Total");
cells["B4"].PutValue("=SUM(B2:B3)");
int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowTotals = true;
// Create globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Call SetTableRowTypeOfTotals with custom name
settings.SetTableRowTypeOfTotals("CustomTotals");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
}
// Save the workbook
workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
