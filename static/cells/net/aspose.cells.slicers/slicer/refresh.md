##Slicer.Refresh
Slicer method. Refreshing the slicer.Meanwhile Refreshing and Calculating relative PivotTables
## Slicer.Refresh method
Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables.
```csharp
public void Refresh()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerMethodRefreshDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Cells["A1"].PutValue("Product");
dataSheet.Cells["A2"].PutValue("Apple");
dataSheet.Cells["A3"].PutValue("Banana");
dataSheet.Cells["B1"].PutValue("Sales");
dataSheet.Cells["B2"].PutValue(100);
dataSheet.Cells["B3"].PutValue(200);
Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
int pivotIndex = pivotSheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
Worksheet slicerSheet = workbook.Worksheets.Add("SlicerSheet");
int slicerIndex = slicerSheet.Slicers.Add(pivotTable, "A1", "Product");
Slicer slicer = slicerSheet.Slicers[slicerIndex];
dataSheet.Cells["A2"].PutValue("Orange");
slicer.Refresh();
workbook.Save("SlicerRefreshDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
