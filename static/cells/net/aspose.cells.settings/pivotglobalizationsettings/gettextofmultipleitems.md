##PivotGlobalizationSettings.GetTextOfMultipleItems
PivotGlobalizationSettings method. Gets the text of Multiple Items label in the PivotTable
## PivotGlobalizationSettings.GetTextOfMultipleItems method
Gets the text of "(Multiple Items)" label in the PivotTable.
```csharp
public virtual string GetTextOfMultipleItems()
```
### Return Value
The text of "(Multiple Items)" label
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B4"].PutValue(3000);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and use globalization settings
PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
// Demonstrate GetTextOfMultipleItems and other key methods
Console.WriteLine("Multiple Items Text: " + settings.GetTextOfMultipleItems());
Console.WriteLine("Total Text: " + settings.GetTextOfTotal());
Console.WriteLine("Grand Total Text: " + settings.GetTextOfGrandTotal());
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
