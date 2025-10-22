##SettablePivotGlobalizationSettings.GetTextOfAll
SettablePivotGlobalizationSettings method. Gets the text of All label in the PivotTable
## SettablePivotGlobalizationSettings.GetTextOfAll method
Gets the text of "(All)" label in the PivotTable.
```csharp
public override string GetTextOfAll()
```
### Return Value
The text of "(All)" label
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(15);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create globalization settings
SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
settings.SetTextOfAll("(All Items)");
try
{
// Get the current text of "(All)" label
string currentText = settings.GetTextOfAll();
Console.WriteLine($"Current text of '(All)' label: {currentText}");
// Refresh pivot table with new settings
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTextOfAllDemo.xlsx");
}
}
}
```
### See Also
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
