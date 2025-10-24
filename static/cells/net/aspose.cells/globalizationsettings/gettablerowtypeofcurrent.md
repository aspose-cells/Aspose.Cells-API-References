##GlobalizationSettings.GetTableRowTypeOfCurrent
GlobalizationSettings method. Gets the type name of table rows that consists of the current row in referenced table. Default is This Row so in formula This Row represents the current row in referenced table
## GlobalizationSettings.GetTableRowTypeOfCurrent method
Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table.
```csharp
public virtual string GetTableRowTypeOfCurrent()
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
public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
// Create sample data and table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
// Create table
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "PriceTable"; // Fixed property name
// Add formula using current row reference
Cell formulaCell = worksheet.Cells["C2"];
formulaCell.Formula = "=PriceTable[@Price] * 1.2";
// Demonstrate the effect of GetTableRowTypeOfCurrent
Console.WriteLine("Generated formula: " + formulaCell.Formula);
Console.WriteLine("Method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetTableRowTypeOfCurrent()
{
return "CurrentItem"; // Custom current row identifier
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
