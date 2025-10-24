##Slicer.AddPivotConnection
Slicer method. Adds PivotTable connection
## Slicer.AddPivotConnection method
Adds PivotTable connection.
```csharp
public void AddPivotConnection(PivotTable pivot)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | The PivotTable object |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerMethodAddPivotConnectionWithPivotTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["B2"].Value = 10;
cells["B3"].Value = 15;
cells["B4"].Value = 5;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add slicer - corrected parameters
int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
Slicer slicer = sheet.Slicers[slicerIndex];
// Add pivot connection to slicer
slicer.AddPivotConnection(pivotTable);
// Save the workbook
workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
