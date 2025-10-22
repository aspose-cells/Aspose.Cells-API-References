##Class CustomPiovtFieldGroupItem
Aspose.Cells.Pivot.CustomPiovtFieldGroupItem class. Represents an item of custom grouped field
## CustomPiovtFieldGroupItem class
Represents an item of custom grouped field.
```csharp
public class CustomPiovtFieldGroupItem
```
## Constructors
| Name | Description |
| --- | --- |
| [CustomPiovtFieldGroupItem](custompiovtfieldgroupitem/)(string, int[]) | The constructor of custom group item of pivot field. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotClassCustomPiovtFieldGroupItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
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
int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);
workbook.Save("PivotClassCustomPiovtFieldGroupItemDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
