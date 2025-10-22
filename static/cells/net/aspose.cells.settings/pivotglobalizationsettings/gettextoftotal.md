##PivotGlobalizationSettings.GetTextOfTotal
PivotGlobalizationSettings method. Gets the text of Total label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area
## PivotGlobalizationSettings.GetTextOfTotal method
Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.
```csharp
public virtual string GetTextOfTotal()
```
### Return Value
The text of "Total" label
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and use globalization settings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfTotal method
Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());
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
