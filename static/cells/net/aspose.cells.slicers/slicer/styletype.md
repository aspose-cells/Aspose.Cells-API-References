##Slicer.StyleType
Slicer property. Specify the type of Builtin slicer style the default type is SlicerStyleLight1
## Slicer.StyleType property
Specify the type of Built-in slicer style the default type is SlicerStyleLight1
```csharp
public SlicerStyleType StyleType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyStyleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["B4"].PutValue(20);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Set slicer properties including StyleType
slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
slicer.Caption = "Fruit Selection";
slicer.NumberOfColumns = 2;
slicer.Width = 200;
slicer.Height = 100;
// Save the workbook
workbook.Save("SlicerStyleTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
