##SettableGlobalizationSettings.GetTableRowTypeOfTotals
SettableGlobalizationSettings method. Gets the type name of table rows that consists of the total row of referenced table
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method
Gets the type name of table rows that consists of the total row of referenced table.
```csharp
public override string GetTableRowTypeOfTotals()
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
public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample table data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["A4"].PutValue("Total");
worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
// Create a ListObject (Table)
int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = worksheet.ListObjects[index];
table.ShowTotals = true;
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
settings.SetTableRowTypeOfTotals("CustomTotals");
try
{
// Get the table row type for totals
string rowType = settings.GetTableRowTypeOfTotals();
Console.WriteLine($"Table row type for totals: {rowType}");
// Apply settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Verify the effect in a formula
worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
