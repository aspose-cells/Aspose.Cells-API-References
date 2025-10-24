##SlicerCollection.RemoveAt
SlicerCollection method. Deletes the Slicer at the specified index
## SlicerCollection.RemoveAt method
Deletes the Slicer at the specified index
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position index in Slicer collection |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
// Add some data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 5;
worksheet.Cells["B4"].Value = 8;
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add slicers
Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
slicers.Add(pivotTable, "Fruit", "FruitSlicer2");
// Remove the second slicer at index 1
slicers.RemoveAt(1);
// Save the workbook
workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
