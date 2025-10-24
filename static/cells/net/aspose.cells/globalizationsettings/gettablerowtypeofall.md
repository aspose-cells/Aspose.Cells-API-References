##GlobalizationSettings.GetTableRowTypeOfAll
GlobalizationSettings method. Gets the type name of table rows that consists of all rows in referenced table. Default is All so in formula All represents all rows in referenced table
## GlobalizationSettings.GetTableRowTypeOfAll method
Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table.
```csharp
public virtual string GetTableRowTypeOfAll()
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
public class CustomGlobalizationSettings2 : GlobalizationSettings
{
public override string GetTableRowTypeOfAll()
{
return "TotalData";
}
}
public class GlobalizationSettingsMethodGetTableRowTypeOfAllDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Qty");
worksheet.Cells["A2"].PutValue("Book");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Pen");
worksheet.Cells["B3"].PutValue(20);
// Convert "A1:B3" to 0-based indices: startRow=0, startColumn=0, endRow=2, endColumn=1
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "Inventory"; // Use DisplayName property instead of Name
CustomGlobalizationSettings2 globalizationSettings = new CustomGlobalizationSettings2();
workbook.Settings.GlobalizationSettings = globalizationSettings;
try
{
string rowType = globalizationSettings.GetTableRowTypeOfAll();
Console.WriteLine($"Table row type for All: {rowType}");
Cell formulaCell = worksheet.Cells["A5"];
formulaCell.Formula = "=SUM(Inventory[#All])";
workbook.CalculateFormula();
Console.WriteLine($"Processed formula: {formulaCell.Formula}");
workbook.Save("GlobalizationSettingsMethodGetTableRowTypeOfAllDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
