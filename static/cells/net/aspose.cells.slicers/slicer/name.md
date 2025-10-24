##Slicer.Name
Slicer property. Returns or sets the name of the specified slicer
## Slicer.Name property
Returns or sets the name of the specified slicer
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Vegetable");
int tableIndex = worksheet.ListObjects.Add("A1", "A3", true);
ListObject table = worksheet.ListObjects[tableIndex];
int slicerIndex = worksheet.Slicers.Add(table, 0, "B1");
Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.Name = "slicer name";
workbook.Save("SlicerPropertyNameDemoOutput.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
