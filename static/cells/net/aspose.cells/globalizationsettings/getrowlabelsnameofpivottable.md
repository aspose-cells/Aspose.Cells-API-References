##GlobalizationSettings.GetRowLabelsNameOfPivotTable
GlobalizationSettings method. Gets the name of Row Labels label in the PivotTable
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method
Gets the name of "Row Labels" label in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```
### Return Value
The name of row labels
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetRowLabelsNameOfPivotTable()
{
return "Custom Row Labels";
}
}
public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["A2"].PutValue("Bikes");
cells["A3"].PutValue("Cars");
cells["B1"].PutValue("Sales");
cells["B2"].PutValue(1000);
cells["B3"].PutValue(2500);
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
// Apply custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Pivot table created with custom row labels name.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
}
workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
