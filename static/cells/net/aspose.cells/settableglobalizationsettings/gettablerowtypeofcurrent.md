##SettableGlobalizationSettings.GetTableRowTypeOfCurrent
SettableGlobalizationSettings method. Gets the type name of table rows that consists of the current row in referenced table
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method
Gets the type name of table rows that consists of the current row in referenced table.
```csharp
public override string GetTableRowTypeOfCurrent()
```
### Return Value
the type name of table rows
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
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
table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
settings.SetTableRowTypeOfCurrent("CurrentRow");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Get the current row type name
string currentRowType = settings.GetTableRowTypeOfCurrent();
Console.WriteLine("Current row type name: " + currentRowType);
// Add a formula referencing the current row
cells["C2"].Formula = "=SUM(#CurrentRow)";
Console.WriteLine("Formula set to: " + cells["C2"].Formula);
// Calculate formulas
workbook.CalculateFormula();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
