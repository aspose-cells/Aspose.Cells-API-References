##Class PivotDiscreteGroupSettings
Aspose.Cells.Pivot.PivotDiscreteGroupSettings class. Rrepsents the discrete group of pivot field
## PivotDiscreteGroupSettings class
Rrepsents the discrete group of pivot field
```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```
## Properties
| Name | Description |
| --- | --- |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | Gets the discrete items. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Gets the group type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotDiscreteGroupSettingsDemo
{
public static void PivotDiscreteGroupSettingsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding some sample data
worksheet.Cells[0, 0].PutValue("Item");
worksheet.Cells[0, 1].PutValue("Quantity");
worksheet.Cells[1, 0].PutValue("A");
worksheet.Cells[1, 1].PutValue(10);
worksheet.Cells[2, 0].PutValue("B");
worksheet.Cells[2, 1].PutValue(15);
worksheet.Cells[3, 0].PutValue("A");
worksheet.Cells[3, 1].PutValue(10);
worksheet.Cells[4, 0].PutValue("B");
worksheet.Cells[4, 1].PutValue(15);
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Set row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Accessing the row field
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);
// Create an instance of PivotDiscreteGroupSettings
PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
// Set the group type to Discrete (This property is read-only)
// Display the current group type
Console.WriteLine("Group Type: " + groupSettings.Type);
// Save the workbook
workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");
return;
}
}
}
```
### See Also
* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
