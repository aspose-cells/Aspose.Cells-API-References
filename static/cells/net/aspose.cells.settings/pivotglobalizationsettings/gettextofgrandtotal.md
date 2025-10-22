##PivotGlobalizationSettings.GetTextOfGrandTotal
PivotGlobalizationSettings method. Gets the text of Grand Total label in the PivotTable
## PivotGlobalizationSettings.GetTextOfGrandTotal method
Gets the text of "Grand Total" label in the PivotTable.
```csharp
public virtual string GetTextOfGrandTotal()
```
### Return Value
The text of "Grand Total" label
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
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
// Create globalization settings and demonstrate GetTextOfGrandTotal
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
Console.WriteLine("Grand Total Text: " + globalizationSettings.GetTextOfGrandTotal());
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
