##GlobalizationSettings.GetPivotTotalName
GlobalizationSettings method. Gets the name of Total label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area
## GlobalizationSettings.GetPivotTotalName method
Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```
### Return Value
The name of "Total" label
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetPivotTotalNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
worksheet.Cells["A1"].Value = "Region";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["C1"].Value = "Quantity";
worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity
// Create and configure globalization settings
var customSettings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = customSettings;
try
{
// Demonstrate direct method call
Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());
// Process pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Pivot table created with custom total name.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetPivotTotalName()
{
return "Custom Total";
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
