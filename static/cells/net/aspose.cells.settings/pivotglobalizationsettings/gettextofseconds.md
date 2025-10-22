##PivotGlobalizationSettings.GetTextOfSeconds
PivotGlobalizationSettings method. Gets the local text of Seconds
## PivotGlobalizationSettings.GetTextOfSeconds method
Gets the local text of "Seconds"
```csharp
public virtual string GetTextOfSeconds()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(DateTime.Now);
worksheet.Cells["B2"].PutValue(100);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add date field to row area
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Create globalization settings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfSeconds method
Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());
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
