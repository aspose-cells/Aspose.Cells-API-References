##PivotDiscreteGroupSettings.Items
PivotDiscreteGroupSettings property. Gets the discrete items
## PivotDiscreteGroupSettings.Items property
Gets the discrete items.
```csharp
public CustomPiovtFieldGroupItem[] Items { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotDiscreteGroupSettingsPropertyItemsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Apple");
worksheet.Cells["A6"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["B5"].PutValue(150);
worksheet.Cells["B6"].PutValue(250);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Get pivot field and group it
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);
// Access discrete group settings
PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
// Display current items
Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
{
Console.WriteLine("Item: " + item.ToString());
}
// Save the workbook
workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
}
}
}
```
### See Also
* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
