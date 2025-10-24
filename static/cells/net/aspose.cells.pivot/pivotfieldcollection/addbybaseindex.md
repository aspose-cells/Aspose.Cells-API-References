##PivotFieldCollection.AddByBaseIndex
PivotFieldCollection method. Adds a PivotField Object to the specific type PivotFields
## PivotFieldCollection.AddByBaseIndex method
Adds a PivotField Object to the specific type PivotFields.
```csharp
public int AddByBaseIndex(int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | field index in the base PivotFields. |
### Return Value
the index of the PivotField Object in this PivotFields.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Banana";
worksheet.Cells["B1"].Value = "Year";
worksheet.Cells["B2"].Value = 2022;
worksheet.Cells["B3"].Value = 2023;
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["C3"].Value = 2000;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add initial fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add Year field to row area using AddByBaseIndex
int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
Console.WriteLine("Added field at index: " + newIndex);
workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
