##PivotFieldCollection.Move
PivotFieldCollection method. Moves the PivotField from current position to destination position
## PivotFieldCollection.Move method
Moves the PivotField from current position to destination position
```csharp
public void Move(int currPos, int destPos)
```
| Parameter | Type | Description |
| --- | --- | --- |
| currPos | Int32 | Current position of PivotField based on zero |
| destPos | Int32 | Destination position of PivotField based on zero |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldCollectionMethodMoveWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["B1"].Value = "Quantity";
cells["B2"].Value = 10;
cells["B3"].Value = 15;
cells["B4"].Value = 20;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to row area
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
Console.WriteLine("Before move:");
for (int i = 0; i < pivotTable.RowFields.Count; i++)
{
Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
}
// Move the first field to position 1
pivotTable.RowFields.Move(0, 1);
Console.WriteLine("\nAfter move:");
for (int i = 0; i < pivotTable.RowFields.Count; i++)
{
Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
}
}
}
}
```
### See Also
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
