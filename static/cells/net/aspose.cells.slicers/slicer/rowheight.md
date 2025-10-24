##Slicer.RowHeight
Slicer property. Returns or sets the height in points of each row in the specified slicer
## Slicer.RowHeight property
Returns or sets the height, in points, of each row in the specified slicer.
```csharp
public double RowHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyRowHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Fruit";
worksheet.Cells["A3"].Value = "Fruit";
worksheet.Cells["A4"].Value = "Vegetable";
int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
int slicerIndex = worksheet.Slicers.Add(pivotTable, "E1", 0);
Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.RowHeight = 20;
workbook.Save("SlicerRowHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
