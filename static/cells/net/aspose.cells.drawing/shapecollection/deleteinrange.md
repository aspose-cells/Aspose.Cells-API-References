##ShapeCollection.DeleteInRange
ShapeCollection method. Delete shapes in the range.Comment shapes will not be deleted
## ShapeCollection.DeleteInRange method
Delete shapes in the range.Comment shapes will not be deleted.
```csharp
public void DeleteInRange(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range.If the shapes are contained in the range, they will be removed. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
// Add first rectangle shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// Add second rectangle shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
// Define the range where shapes should be deleted
CellArea area = new CellArea();
area.StartColumn = 0;
area.StartRow = 5;
area.EndColumn = 5;
area.EndRow = 8;
// Delete shapes within the specified range
shapes.DeleteInRange(area);
// Save the workbook (optional)
workbook.Save("ShapeDeleteInRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
