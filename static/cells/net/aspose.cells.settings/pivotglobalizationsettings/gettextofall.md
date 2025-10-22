##PivotGlobalizationSettings.GetTextOfAll
PivotGlobalizationSettings method. Gets the text of All label in the PivotTable
## PivotGlobalizationSettings.GetTextOfAll method
Gets the text of "(All)" label in the PivotTable.
```csharp
public virtual string GetTextOfAll()
```
### Return Value
The text of "(All)" label
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
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
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["B3"].PutValue(2000);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and use globalization settings
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfAll method
Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
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
