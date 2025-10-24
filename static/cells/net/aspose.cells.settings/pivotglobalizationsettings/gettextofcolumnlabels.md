##PivotGlobalizationSettings.GetTextOfColumnLabels
PivotGlobalizationSettings method. Gets the text of Column Labels label in the PivotTable
## PivotGlobalizationSettings.GetTextOfColumnLabels method
Gets the text of "Column Labels" label in the PivotTable.
```csharp
public virtual string GetTextOfColumnLabels()
```
### Return Value
The text of column labels
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(800);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and use globalization settings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfColumnLabels
Console.WriteLine("Column Labels Text: " + globalizationSettings.GetTextOfColumnLabels());
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
