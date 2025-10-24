##SettableGlobalizationSettings.SetTableRowTypeOfData
SettableGlobalizationSettings method. Sets the type name of table rows that consists of data region of referenced table
## SettableGlobalizationSettings.SetTableRowTypeOfData method
Sets the type name of table rows that consists of data region of referenced table.
```csharp
public void SetTableRowTypeOfData(string name)
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
public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
cells["A2"].PutValue("John");
cells["B2"].PutValue(30);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(25);
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowTotals = true;
table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;
// Create globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Set custom name for data rows in table
settings.SetTableRowTypeOfData("MyDataRegion");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
Console.WriteLine("Table row type of data set to: MyDataRegion");
Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
}
// Save the workbook
workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
