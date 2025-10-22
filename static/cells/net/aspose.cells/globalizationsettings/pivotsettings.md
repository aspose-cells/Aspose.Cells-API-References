##GlobalizationSettings.PivotSettings
GlobalizationSettings property. Gets or sets the globalization settings for pivot table
## GlobalizationSettings.PivotSettings property
Gets or sets the globalization settings for pivot table.
```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
{
public override string GetTextOfTotal()
{
return "Custom Total";
}
public override string GetTextOfGrandTotal()
{
return "Custom Grand Total";
}
public override string GetTextOfDataFieldHeader()
{
return "DataCaption";
}
public override string GetTextOfProtectedName(string protectedName)
{
return protectedName + "2";
}
}
public class GlobalizationSettingsPropertyPivotSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Cells["A1"].PutValue("Product");
dataSheet.Cells["B1"].PutValue("Sales");
dataSheet.Cells["A2"].PutValue("Apple");
dataSheet.Cells["B2"].PutValue(1000);
dataSheet.Cells["A3"].PutValue("Orange");
dataSheet.Cells["B3"].PutValue(2000);
// Create pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Set custom globalization settings for pivot table
CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;
// Refresh pivot table to apply settings
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotGlobalizationDemo.xlsx");
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
