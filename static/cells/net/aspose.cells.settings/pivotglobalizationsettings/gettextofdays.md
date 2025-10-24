##PivotGlobalizationSettings.GetTextOfDays
PivotGlobalizationSettings method. Gets the local text of Days
## PivotGlobalizationSettings.GetTextOfDays method
Gets the local text of "Days".
```csharp
public virtual string GetTextOfDays()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue(DateTime.Now);
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
worksheet.Cells["B3"].PutValue(1500);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add date field to row area
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Create globalization settings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfDays method
Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());
// Save the workbook
workbook.Save("PivotGlobalizationDemo.xlsx");
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
