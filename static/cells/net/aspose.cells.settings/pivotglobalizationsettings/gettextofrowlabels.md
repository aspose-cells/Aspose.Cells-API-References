##PivotGlobalizationSettings.GetTextOfRowLabels
PivotGlobalizationSettings method. Gets the text of Row Labels label in the PivotTable
## PivotGlobalizationSettings.GetTextOfRowLabels method
Gets the text of "Row Labels" label in the PivotTable.
```csharp
public virtual string GetTextOfRowLabels()
```
### Return Value
The text of row labels
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Vegetable");
worksheet.Cells["B3"].PutValue(200);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and use globalization settings
PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfRowLabels
Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());
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
