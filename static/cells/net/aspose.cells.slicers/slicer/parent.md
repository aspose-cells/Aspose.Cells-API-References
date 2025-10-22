##Slicer.Parent
Slicer property. Returns the Worksheet object which contains this slicer. Readonly
## Slicer.Parent property
Returns the [`Worksheet`](../../../aspose.cells/worksheet/) object which contains this slicer. Read-only.
```csharp
public Worksheet Parent { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyParentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
int tableIndex = sheet.ListObjects.Add("A1", "A4", true);
ListObject table = sheet.ListObjects[tableIndex];
int slicerIndex = sheet.Slicers.Add(table, 0, "B1");
Slicer slicer = sheet.Slicers[slicerIndex];
Worksheet currSheet = slicer.Parent;
currSheet.Cells["C1"].Value = "ParentWorksheetAccessed";
workbook.Save("SlicerParentDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
