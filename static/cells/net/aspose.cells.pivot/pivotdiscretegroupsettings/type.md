##PivotDiscreteGroupSettings.Type
PivotDiscreteGroupSettings property. Gets the group type
## PivotDiscreteGroupSettings.Type property
Gets the group type.
```csharp
public override PivotFieldGroupType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotDiscreteGroupSettingsPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells[0, 0].PutValue("Item");
worksheet.Cells[0, 1].PutValue("Value");
worksheet.Cells[1, 0].PutValue("A");
worksheet.Cells[1, 1].PutValue(10);
worksheet.Cells[2, 0].PutValue("B");
worksheet.Cells[2, 1].PutValue(20);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Group items
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(new CustomPiovtFieldGroupItem[] {
new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 })
}, true);
// Get group settings and demonstrate Type property
PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
Console.WriteLine("Group Type: " + groupSettings.Type);
workbook.Save("PivotDiscreteGroupSettingsDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
